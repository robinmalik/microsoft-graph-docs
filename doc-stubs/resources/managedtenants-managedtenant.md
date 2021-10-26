---
title: "managedTenant resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managedTenant resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/managedtenants-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedTenants](../api/managedtenants-managedtenant-list.md)|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md) collection|Get a list of the [managedTenant](../resources/managedtenants-managedtenant.md) objects and their properties.|
|[Create managedTenant](../api/managedtenants-tenantrelationship-post-managedtenants.md)|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|Create a new [managedTenant](../resources/managedtenants-managedtenant.md) object.|
|[Get managedTenant](../api/managedtenants-managedtenant-get.md)|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|Read the properties and relationships of a [managedTenant](../resources/managedtenants-managedtenant.md) object.|
|[Update managedTenant](../api/managedtenants-managedtenant-update.md)|[microsoft.graph.managedTenants.managedTenant](../resources/managedtenants-managedtenant.md)|Update the properties of a [managedTenant](../resources/managedtenants-managedtenant.md) object.|
|[Delete managedTenant](../api/managedtenants-managedtenant-delete.md)|None|Deletes a [managedTenant](../resources/managedtenants-managedtenant.md) object.|
|[List managementTemplateCollections](../api/managedtenants-managedtenant-list-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get the managementTemplateCollection resources from the managementTemplateCollections navigation property.|
|[Create managementTemplateCollection](../api/managedtenants-managedtenant-post-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Create a new managementTemplateCollection object.|
|[List managementTemplateSteps](../api/managedtenants-managedtenant-list-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get the managementTemplateStep resources from the managementTemplateSteps navigation property.|
|[Create managementTemplateStep](../api/managedtenants-managedtenant-post-managementtemplatesteps.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Create a new managementTemplateStep object.|
|[List managementTemplateStepVersions](../api/managedtenants-managedtenant-list-managementtemplatestepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the managementTemplateStepVersion resources from the managementTemplateStepVersions navigation property.|
|[Create managementTemplateStepVersion](../api/managedtenants-managedtenant-post-managementtemplatestepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md)|Create a new managementTemplateStepVersion object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|aggregatedPolicyCompliances|[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) collection|**TODO: Add Description**|
|cloudPcConnections|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) collection|**TODO: Add Description**|
|cloudPcDevices|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) collection|**TODO: Add Description**|
|cloudPcsOverview|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) collection|**TODO: Add Description**|
|conditionalAccessPolicyCoverages|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) collection|**TODO: Add Description**|
|credentialUserRegistrationsSummaries|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) collection|**TODO: Add Description**|
|deviceCompliancePolicySettingStateSummaries|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-intune-devicecompliancepolicysettingstatesummary.md) collection|**TODO: Add Description**|
|managedDeviceCompliances|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) collection|**TODO: Add Description**|
|managedDeviceComplianceTrends|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) collection|**TODO: Add Description**|
|managementActions|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) collection|**TODO: Add Description**|
|managementActionTenantDeploymentStatuses|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) collection|**TODO: Add Description**|
|managementIntents|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) collection|**TODO: Add Description**|
|managementTemplateCollections|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|**TODO: Add Description**|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|**TODO: Add Description**|
|managementTemplateSteps|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|**TODO: Add Description**|
|managementTemplateStepVersions|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|**TODO: Add Description**|
|tenantGroups|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection|**TODO: Add Description**|
|tenants|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) collection|**TODO: Add Description**|
|tenantsCustomizedInformation|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection|**TODO: Add Description**|
|tenantsDetailedInformation|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) collection|**TODO: Add Description**|
|tenantTags|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) collection|**TODO: Add Description**|
|windowsDeviceMalwareStates|[microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-intune-windowsdevicemalwarestate.md) collection|**TODO: Add Description**|
|windowsProtectionStates|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-intune-windowsprotectionstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedTenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenant",
  "id": "String (identifier)"
}
```

