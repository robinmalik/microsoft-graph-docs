---
title: "synchronizationQuarantine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationQuarantine resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentBegan|DateTimeOffset|**TODO: Add Description**|
|error|[synchronizationError](../resources/synchronizationerror.md)|**TODO: Add Description**|
|nextAttempt|DateTimeOffset|**TODO: Add Description**|
|reason|quarantineReason|**TODO: Add Description**. The possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`, `QuarantinedOnDemand`, `TooManyDeletes`, `IngestionInterrupted`.|
|seriesBegan|DateTimeOffset|**TODO: Add Description**|
|seriesCount|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationQuarantine",
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "error": {
    "@odata.type": "microsoft.graph.synchronizationError"
  },
  "seriesBegan": "String (timestamp)",
  "seriesCount": "Integer"
}
```

