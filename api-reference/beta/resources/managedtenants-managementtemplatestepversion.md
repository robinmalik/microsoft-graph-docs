---
title: "managementTemplateStepVersion resource type"
description: "Represents details for the management template step version."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStepVersion resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents details for the management template step version.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateStepVersions](../api/managedtenants-managementtemplatestepversion-list.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get a list of the [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) objects and their properties.|
|[Get managementTemplateStepVersion](../api/managedtenants-managementtemplatestepversion-get.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Read the properties and relationships of a [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.|
|[deploy](../api/managedtenants-managementtemplatestepversion-deploy.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Deploys the management template step to the specified managed tenant.|
|[List deployments](../api/managedtenants-managementtemplatestepversion-list-deployments.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|Get the managementTemplateStepDeployment resources from the deployments navigation property.|
|[List managementTemplateStep](../api/managedtenants-managementtemplatestepversion-list-templatestep.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get the managementTemplateStep resources from the templateStep navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configurationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|The action to be performed when applying the management template step. Required. Read-only.|
|id|String|The unique identifier for the management template step version. Required. Read-only.|
|validationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|The action that will be used to validate the created artifacts are still presented. Required. Read-only.|
|version|Int32|The version for the management template step. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deployments|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|The collection of deployments associated with the management template step version.|
|templateStep|[managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|The template step associated with this management template step version.|

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
