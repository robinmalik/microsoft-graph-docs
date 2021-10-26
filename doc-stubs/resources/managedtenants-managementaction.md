---
title: "managementAction resource type"
description: "Represents a management action that will be performed on behalf of a managed tenant."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementAction resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a management action that will be performed on behalf of a managed tenant.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementActions](../api/managedtenants-managementaction-list.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) collection|Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.|
|[Get managementAction](../api/managedtenants-managementaction-get.md)|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.|
|[apply](../api/managedtenants-managementaction-apply.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|Applies the management action to a given managed tenant.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|The type of category for this management action. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`. Optional. Read-only.|
|description|String|This description for this management action. Optional. Read-only.|
|displayName|String|The display name for this management action. Optional. Read-only.|
|id|String|The unique identifier for this management action. Required. Read-only.|
|referenceTemplateId|String|The unique identifier for the reference management template. Required. Read-only.|
|referenceTemplateVersion|Int32|The version of the reference management template. Required. Read-only.|
|workloadActions|[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection|The collection of workload actions associated with the management action. Required. Read-only.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementAction",
  "id": "String (identifier)",
  "referenceTemplateId": "String",
  "referenceTemplateVersion": "Integer",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
