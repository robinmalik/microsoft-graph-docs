---
title: "managementTemplate resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplate resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/managedtenants-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplates](../api/managedtenants-managementtemplate-list.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.|
|[Create managementTemplate](../api/managedtenants-managedtenant-post-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Create a new [managementTemplate](../resources/managedtenants-managementtemplate.md) object.|
|[Get managementTemplate](../api/managedtenants-managementtemplate-get.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.|
|[Update managementTemplate](../api/managedtenants-managementtemplate-update.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Update the properties of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.|
|[Delete managementTemplate](../api/managedtenants-managementtemplate-delete.md)|None|Deletes a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.|
|[List managementTemplateCollections](../api/managedtenants-managementtemplate-list-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get the managementTemplateCollection resources from the managementTemplateCollections navigation property.|
|[Add managementTemplateCollection](../api/managedtenants-managementtemplate-post-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Add managementTemplateCollections by posting to the managementTemplateCollections collection.|
|[List managementTemplateSteps](../api/managedtenants-managementtemplate-list-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get the managementTemplateStep resources from the managementTemplateSteps navigation property.|
|[Add managementTemplateStep](../api/managedtenants-managementtemplate-post-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Add managementTemplateSteps by posting to the managementTemplateSteps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|**TODO: Add Description**. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|parameters|[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) collection|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|
|workloadActions|[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplateCollections|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|**TODO: Add Description**|
|managementTemplateSteps|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|**TODO: Add Description**|

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

