---
title: "managementTemplateStepVersion resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStepVersion resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/managedtenants-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateStepVersions](../api/managedtenants-managementtemplatestepversion-list.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get a list of the [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) objects and their properties.|
|[Create managementTemplateStepVersion](../api/managedtenants-managementtemplatestep-post-stepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Create a new [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[Get managementTemplateStepVersion](../api/managedtenants-managementtemplatestepversion-get.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Read the properties and relationships of a [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[Update managementTemplateStepVersion](../api/managedtenants-managementtemplatestepversion-update.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Update the properties of a [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[Delete managementTemplateStepVersion](../api/managedtenants-managementtemplatestepversion-delete.md)|None|Deletes a [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[deploy](../api/managedtenants-managementtemplatestepversion-deploy.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|**TODO: Add Description**|
|[List deployments](../api/managedtenants-managementtemplatestepversion-list-deployments.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|Get the managementTemplateStepDeployment resources from the deployments navigation property.|
|[Add managementTemplateStepDeployment](../api/managedtenants-managementtemplatestepversion-post-deployments.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Add deployments by posting to the deployments collection.|
|[List managementTemplateStep](../api/managedtenants-managementtemplatestepversion-list-templatestep.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get the managementTemplateStep resources from the templateStep navigation property.|
|[Add managementTemplateStep](../api/managedtenants-managementtemplatestepversion-post-templatestep.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Add templateStep by posting to the templateStep collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|validationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deployments|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|**TODO: Add Description**|
|templateStep|[managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepVersion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepVersion",
  "id": "String (identifier)",
  "configurationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "validationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "version": "Integer"
}
```

