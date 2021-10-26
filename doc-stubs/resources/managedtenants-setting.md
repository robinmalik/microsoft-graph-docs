---
title: "setting resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# setting resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|jsonValue|String|**TODO: Add Description**|
|overwriteAllowed|Boolean|**TODO: Add Description**|
|settingId|String|**TODO: Add Description**|
|valueType|managementParameterValueType|**TODO: Add Description**. The possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.|

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

