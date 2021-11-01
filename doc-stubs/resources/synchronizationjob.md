---
title: "synchronizationJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationJob resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizationJobs](../api/synchronizationjob-list.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get a list of the [synchronizationJob](../resources/synchronizationjob.md) objects and their properties.|
|[Create synchronizationJob](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Create a new [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Get synchronizationJob](../api/synchronizationjob-get.md)|[synchronizationJob](../resources/synchronizationjob.md)|Read the properties and relationships of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Update synchronizationJob](../api/synchronizationjob-update.md)|[synchronizationJob](../resources/synchronizationjob.md)|Update the properties of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Delete synchronizationJob](../api/synchronizationjob-delete.md)|None|Deletes a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[pause](../api/synchronizationjob-pause.md)|None|**TODO: Add Description**|
|[provisionOnDemand](../api/synchronizationjob-provisionondemand.md)|[stringKeyStringValuePair](../resources/stringkeystringvaluepair.md)|**TODO: Add Description**|
|[start](../api/synchronizationjob-start.md)|None|**TODO: Add Description**|
|[stop](../api/synchronizationjob-stop.md)|None|**TODO: Add Description**|
|[restart](../api/synchronizationjob-restart.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[List synchronizationSchema](../api/synchronizationjob-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchema resources from the schema navigation property.|
|[Create synchronizationSchema](../api/synchronizationjob-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new synchronizationSchema object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)|**TODO: Add Description**|
|status|[synchronizationStatus](../resources/synchronizationstatus.md)|**TODO: Add Description**|
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "String (identifier)",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule"
  },
  "status": {
    "@odata.type": "microsoft.graph.synchronizationStatus"
  },
  "templateId": "String",
  "synchronizationJobSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

