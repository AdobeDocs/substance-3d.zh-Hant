---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-scripting.html"
breadcrumb-title: ''
description: 使用 Substance Maya API 來撰寫 Substance 材質的腳本，並在你的 Maya 工作流程中進行管理。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 腳本
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# Maya 腳本

Substance in Maya 插件可以用腳本來寫。一個公開的 API 允許在腳本中使用 Substance 指令來建立和管理 Substance 材料。 你可以透過外掛資訊來存取可用的指令。

***在 Windows>設定/偏好設定/插件管理器中搜尋 substancemaya.mll 檔案。***

點擊「i」按鈕即可查看可用的指令

![](../../../assets/script-7.png)

## 範例腳本：

這個腳本會載入 sbsar 檔案，並將 Arnold 渲染工作流程套用到所選的網格上。 要使用該腳本，請依照此處列出的範例操作。

1. 將程式碼複製貼上到腳本編輯器的 Python 分頁中。
1. 在視窗中選取並網格
1. 在 Python 標籤頁選擇文字，然後按下「ctrl + enter」
1. 在視窗中瀏覽 SBSAR 檔案。

```
import maya.cmds as cmds 

 

def _connect_place2d(substance_node): 

    """ Connects the place2d texture node to the Substance node """ 

    place_node = cmds.shadingNode('place2dTexture', asUtility=True) 

 

    connect_attrs = [('outUV', 'uvCoord'), ('outUvFilterSize', 'uvFilterSize')] 

 

    for out_attr, in_attr in connect_attrs: 

        cmds.connectAttr('{}.{}'.format(place_node, out_attr), 

                         '{}.{}'.format(substance_node, in_attr)) 

 

def _find_shading_group(node): 

    """ Walks the shader graph to find the shading group """ 

    result = None 

 

    connections = cmds.listConnections(node, source=False) 

 

    if connections: 

        for connection in connections: 

            if cmds.nodeType(connection) == 'shadingEngine': 

                result = connection 

            else: 

                result = _find_shading_group(connection) 

                if result is not None: 

                    break 

 

    return result 

 

def _apply_substance_workflow_to_selected(substance_file, workflow): 

    """ Imports a mesh into Maya and applies the shader from a 

        Substance workflow to it """ 

    geometry = cmds.ls(geometry=True) 

 

## Create the substance node and connect the place2d texture node

    substance_node = cmds.shadingNode('substanceNode', asTexture=True) 

    _connect_place2d(substance_node) 

 

## Load the Substance file

    cmds.substanceNodeLoadSubstance(substance_node, substance_file) 

 

## Apply the workflow

    cmds.substanceNodeApplyWorkflow(substance_node, workflow=workflow) 

 

## Acquire the shading group and apply it to the mesh

    shading_group = _find_shading_group(substance_node) 

 

    cmds.select(geometry) 

    cmds.hyperShade(assign=shading_group) 

 

def demo_load_sbsar_workflow(): 

    """ Acquires an sbsar from a file dialog, loading and applying it to 

        any selected mesh """ 

    file_filter = 'Substance (*.sbsar);;' 

 

    files = cmds.fileDialog2(cap='Select a Substance file', fm=1, dialogStyle=2, 

                             okc='Open', fileFilter=file_filter) 

 

    if files: 

        substance_file = files[0] 

        _apply_substance_workflow_to_selected(substance_file, 

                                              cmds.substanceGetWorkflow()) 

 

if __name__ == '__main__': 

    demo_load_sbsar_workflow()
```


一個公開的 API 允許在腳本中使用 Substance 指令
