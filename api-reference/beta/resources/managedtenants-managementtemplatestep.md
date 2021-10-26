---
title: "managementTemplateStep resource type"
description: "Represents a step in management template."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateStep resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a step in management template.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateSteps](../api/managedtenants-managementtemplatestep-list.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) collection|Get a list of the [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) objects and their properties.|
|[Get managementTemplateStep](../api/managedtenants-managementtemplatestep-get.md)|[microsoft.graph.managedTenants.managementTemplateStep](../resources/managedtenants-managementtemplatestep.md)|Read the properties and relationships of a [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.|
|[List managementTemplate](../api/managedtenants-managementtemplatestep-list-managementtemplate.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the managementTemplate resources from the managementTemplate navigation property.|
|[List stepVersions](../api/managedtenants-managementtemplatestep-list-stepversions.md)|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|Get the managementTemplateStepVersion resources from the stepVersions navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|managementCategory|The management category the step. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`. Required. Read-only.|
|description|String|The description for the management template step. Optional. Read-only.|
|displayName|String|The display name for the management template step. Optional. Read-only.|
|id|String|The unique identifier for the management template step. Optional. Read-only.|
|managementPortal|String|The display name for the workload management portal associated with this management template step. Required.|
|portalLink|String|The workload management portal link associated with this management template step. Required.|
|priority|Int32|The position in the sequence this management template step should be performed. Required.|
|provider|managementProvider|The provider for this management template step. The possible values are: `microsoft`, `community`, `indirectProvider`, `self`, `unknownFutureValue`. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplate|[managementTemplate](../resources/managedtenants-managementtemplate.md)|The management template associated with this management template step.|
|stepVersions|[microsoft.graph.managedTenants.managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) collection|The collection of version associated with this management template step.|

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
