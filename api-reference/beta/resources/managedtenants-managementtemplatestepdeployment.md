---
title: "managementTemplateStepDeployment resource type"
description: "Represent the user reported deployment status for a management template step."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStepDeployment resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represent the user reported deployment status for a management template step.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateStepDeployments](../api/managedtenants-managementtemplatestepdeployment-list.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) collection|Get a list of the [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) objects and their properties.|
|[Get managementTemplateStepDeployment](../api/managedtenants-managementtemplatestepdeployment-get.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Read the properties and relationships of a [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) object.|
|[changeDeploymentStatus](../api/managedtenants-managementtemplatestepdeployment-changedeploymentstatus.md)|[microsoft.graph.managedTenants.managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md)|Changes the deployment status for this management template step.|
|[List managementTemplateStepVersion](../api/managedtenants-managementtemplatestepdeployment-list-templatestepversion.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the managementTemplateStepVersion resources from the templateStepVersion navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[microsoft.graph.managedTenants.graphAPIErrorDetails](../resources/managedtenants-graphapierrordetails.md)|The error details for any exception that was encountered when applying the management template step. Optional. Read-only.|
|id|String|The unique identifier for the management template step deployment. Required. Read-only.|
|settings|[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection|The collection of settings associated with this management template step deployment. Optional. Read-only.|
|status|managementTemplateDeploymentStatus|The status for the management template step deployment. The possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`. Required.|
|tenantId|String|The identifier of the tenant associated with this management template step deployment. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|templateStepVersion|[managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|The details for the deployed management template step. Required. Read-only.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepDeployment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepDeployment",
  "id": "String (identifier)",
  "tenantId": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ],
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.managedTenants.graphAPIErrorDetails"
  }
}
```
