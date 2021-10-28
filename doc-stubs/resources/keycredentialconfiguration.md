---
title: "keyCredentialConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# keyCredentialConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maxLifetime|Duration|**TODO: Add Description**|
|restrictForAppsCreatedAfterDateTime|DateTimeOffset|**TODO: Add Description**|
|restrictionType|appKeyCredentialRestrictionType|**TODO: Add Description**. The possible values are: `asymmetricKeyLifetime`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyCredentialConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyCredentialConfiguration",
  "restrictionType": "String",
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "String (timestamp)"
}
```

