---
title: "templateAction resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# templateAction resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|service|String|**TODO: Add Description**|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|**TODO: Add Description**|
|templateActionId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|licenses|[licenseDetails](../resources/managedtenants-licensedetails.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateAction",
  "templateActionId": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```

