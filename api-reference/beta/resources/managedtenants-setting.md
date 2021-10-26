---
title: "setting resource type"
description: "Represents a setting that is part of a template action."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# setting resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a setting that is part of a template action.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name for this setting. Required. Read-only.|
|jsonValue|String|The value for this setting represented as a JSON serialized string. Required. Read-only.|
|overwriteAllowed|Boolean|A flag that indicated whether the setting can be overwritten. Required. Read-only.|
|settingId|String|The identifier for the setting. Required. Read-only.|
|valueType|managementParameterValueType|The type of value this setting represents. The possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Required. Read-only.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "settingId": "String",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```

