---
title: "templateAction resource type"
description: "Represents an action that is part of a template."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# templateAction resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an action that is part of a template.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description for the template action. Optional. Read-only.|
|displayName|String|The display name for the template action. Optional. Read-only.|
|service|String|The workload associated with this template action. Optional. Read-only.|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|The collection of settings associated with the template action. Optional. Read-only.|
|templateActionId|String|The unique identifier for the template action. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|licenses|[licenseDetails](../resources/managedtenants-licensedetails.md)|Details for the license required for this template action.|

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
