---
title: "managementTemplateStep resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managementTemplateStep resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/managedtenants-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateSteps](../api/managedtenants-managementtemplatestep-list.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get a list of the [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) objects and their properties.|
|[Create managementTemplateStep](../api/managedtenants-managementtemplate-post-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Create a new [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[Get managementTemplateStep](../api/managedtenants-managementtemplatestep-get.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Read the properties and relationships of a [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[Update managementTemplateStep](../api/managedtenants-managementtemplatestep-update.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Update the properties of a [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[Delete managementTemplateStep](../api/managedtenants-managementtemplatestep-delete.md)|None|Deletes a [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[List managementTemplate](../api/managedtenants-managementtemplatestep-list-managementtemplate.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the managementTemplate resources from the managementTemplate navigation property.|
|[Add managementTemplate](../api/managedtenants-managementtemplatestep-post-managementtemplate.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Add managementTemplate by posting to the managementTemplate collection.|
|[List stepVersions](../api/managedtenants-managementtemplatestep-list-stepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the managementTemplateStepVersion resources from the stepVersions navigation property.|
|[Add managementTemplateStepVersion](../api/managedtenants-managementtemplatestep-post-stepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Add stepVersions by posting to the stepVersions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|**TODO: Add Description**. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md).|
|managementPortal|String|**TODO: Add Description**|
|portalLink|String|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|provider|managementProvider|**TODO: Add Description**. The possible values are: `microsoft`, `community`, `indirectProvider`, `self`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplate|[managementTemplate](../resources/managedtenants-managementtemplate.md)|**TODO: Add Description**|
|stepVersions|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStep",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStep",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "category": "String",
  "provider": "String",
  "managementPortal": "String",
  "portalLink": "String"
}
```

