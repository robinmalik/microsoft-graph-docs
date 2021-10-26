---
title: "workloadActionDeploymentStatus resource type"
description: "Represents the deployment status for the workload action."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# workloadActionDeploymentStatus resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the deployment status for the workload action.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionId|String|The unique identifier for the workload action. Required. Read-only.|
|deployedPolicyId|String|The identifier of any policy that was created by applying the workload action. Optional. Read-only.|
|error|[microsoft.graph.genericError](../resources/managedtenants-genericerror.md)|The detailed information for exceptions that occur when deploying the workload action. Optional. Required.|
|excludeGroups|String collection|The collection of Azure Active Directory groups that are excluded from the workload action deployment. Optional. Read-only.|
|includeAllUsers|Boolean|A flag that indicates whether all users are included for the workload action deployment. Required. Read-only.|
|includeGroups|String collection|The collection of Azure Active Directory groups that are included from the workload action deployment. Optional. Read-only.|
|lastDeploymentDateTime|DateTimeOffset|The date and time this workload action was last deployed. Optional.|
|status|workloadActionStatus|The status for this workload action deployment. The possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`. Required. Read-only.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)",
  "includeAllUsers": "Boolean",
  "includeGroups": [
    "String"
  ],
  "excludeGroups": [
    "String"
  ]
}
```
