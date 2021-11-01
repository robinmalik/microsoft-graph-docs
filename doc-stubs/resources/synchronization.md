---
title: "synchronization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronization resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizations](../api/synchronization-list.md)|[synchronization](../resources/synchronization.md) collection|Get a list of the [synchronization](../resources/synchronization.md) objects and their properties.|
|[Create synchronization](../api/serviceprincipal-post-synchronization.md)|[synchronization](../resources/synchronization.md)|Create a new [synchronization](../resources/synchronization.md) object.|
|[Get synchronization](../api/synchronization-get.md)|[synchronization](../resources/synchronization.md)|Read the properties and relationships of a [synchronization](../resources/synchronization.md) object.|
|[Update synchronization](../api/synchronization-update.md)|[synchronization](../resources/synchronization.md)|Update the properties of a [synchronization](../resources/synchronization.md) object.|
|[Delete synchronization](../api/synchronization-delete.md)|None|Deletes a [synchronization](../resources/synchronization.md) object.|
|[Ping](../api/synchronization-ping.md)|String|**TODO: Add Description**|
|[acquireAccessToken](../api/synchronization-acquireaccesstoken.md)|None|**TODO: Add Description**|
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get the synchronizationJob resources from the jobs navigation property.|
|[Create synchronizationJob](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Create a new synchronizationJob object.|
|[List templates](../api/synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|Get the synchronizationTemplate resources from the templates navigation property.|
|[Create synchronizationTemplate](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Create a new synchronizationTemplate object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationsecretkeystringvaluepair.md) collection|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|jobs|[synchronizationJob](../resources/synchronizationjob.md) collection|**TODO: Add Description**|
|templates|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronization",
  "version": "String",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

