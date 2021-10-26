---
title: "managementTemplateStepDeployment: changeDeploymentStatus"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: apiPageType
---

# managementTemplateStepDeployment: changeDeploymentStatus
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ManagedTenants.Read.All, ManagedTenants.WriteRead.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}/managementTemplateSteps/{managementTemplateStepId}/stepVersions/{managementTemplateStepVersionId}/deployments/{managementTemplateStepDeploymentId}/changeDeploymentStatus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|tenantId|String|**TODO: Add Description**|
|managementTemplateStepId|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [managementTemplateStepDeployment](../resources/managedtenants-managementtemplatestepdeployment.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "managementtemplatestepdeployment_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}/managementTemplateSteps/{managementTemplateStepId}/stepVersions/{managementTemplateStepVersionId}/deployments/{managementTemplateStepDeploymentId}/changeDeploymentStatus
Content-Type: application/json
Content-length: 92

{
  "tenantId": "String",
  "managementTemplateStepId": "String",
  "status": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepDeployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

