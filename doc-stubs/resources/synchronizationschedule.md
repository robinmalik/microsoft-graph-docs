---
title: "synchronizationSchedule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationSchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiration|DateTimeOffset|**TODO: Add Description**|
|interval|Duration|**TODO: Add Description**|
|state|synchronizationScheduleState|**TODO: Add Description**. The possible values are: `Active`, `Disabled`, `Paused`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchedule",
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}
```

