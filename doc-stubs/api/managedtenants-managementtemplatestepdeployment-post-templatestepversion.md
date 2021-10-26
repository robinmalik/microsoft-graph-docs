---
title: "Add managementTemplateStepVersion"
description: "Add templateStepVersion by posting to the templateStepVersion collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add managementTemplateStepVersion
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add templateStepVersion by posting to the templateStepVersion collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}/managementTemplateSteps/{managementTemplateStepId}/stepVersions/{managementTemplateStepVersionId}/deployments/{managementTemplateStepDeploymentId}/templateStepVersion/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object.

You can specify the following properties when creating a **managementTemplateStepVersion**.

|Property|Type|Description|
|:---|:---|:---|
|configurationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|**TODO: Add Description** Optional.|
|validationAction|[microsoft.graph.managedTenants.templateAction](../resources/managedtenants-templateaction.md)|**TODO: Add Description** Optional.|
|version|Int32|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `204 No Content` response code and a [managementTemplateStepVersion](../resources/managedtenants-managementtemplatestepversion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managementtemplatestepversion_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}/managementTemplateSteps/{managementTemplateStepId}/stepVersions/{managementTemplateStepVersionId}/deployments/{managementTemplateStepDeploymentId}/templateStepVersion/$ref
Content-Type: application/json
Content-length: 312

{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepVersion",
  "configurationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "validationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "version": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStepVersion"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStepVersion",
  "id": "77214605-4605-7721-0546-217705462177",
  "configurationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "validationAction": {
    "@odata.type": "microsoft.graph.managedTenants.templateAction"
  },
  "version": "Integer"
}
```

