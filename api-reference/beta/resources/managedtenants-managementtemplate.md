---
title: "managementTemplate resource type"
description: "Represents a group of actions and settings used to perform a set of actions or configurations for a given managed tenant."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplate resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a group of actions and settings used to perform a set of actions or configurations for a given managed tenant.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplates](../api/managedtenants-managementtemplate-list.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.|
|[Get managementTemplate](../api/managedtenants-managementtemplate-get.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.|
|[List managementTemplateCollections](../api/managedtenants-managementtemplate-list-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get the managementTemplateCollection resources from the managementTemplateCollections navigation property.|
|[List managementTemplateSteps](../api/managedtenants-managementtemplate-list-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get the managementTemplateStep resources from the managementTemplateSteps navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|The management category for the management template. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`. Required. Read-only.|
|description|String|The description for the management template. Optional. Read-only.|
|displayName|String|The display name for the management template. Required. Read-only.|
|id|String|The unique identifier for the management template. Required. Read-only.|
|parameters|[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) collection|The collection of parameters used by the management template. Optional. Read-only.|
|version|Int32|The version for the management template. Required. Read-only.|
|workloadActions|[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection|The collection of workload actions associated with the management template. Optional. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplateCollections|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|The management template collection available across managed tenants.|
|managementTemplateSteps|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|The collection of step included in this management template.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "version": "Integer",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
