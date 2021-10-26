---
title: "Create managementTemplateStep"
description: "Create a new managementTemplateStep object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managementTemplateStep
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new managementTemplateStep object.

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
POST /tenantRelationships/managedTenants/managementTemplateSteps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object.

You can specify the following properties when creating a **managementTemplateStep**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|priority|Int32|**TODO: Add Description** Optional.|
|category|managementCategory|**TODO: Add Description**. The possible values are: `custom`, `devices`, `identity`, `data`, `unknownFutureValue`. Optional.|
|provider|managementProvider|**TODO: Add Description**. The possible values are: `microsoft`, `community`, `indirectProvider`, `self`, `unknownFutureValue`. Optional.|
|managementPortal|String|**TODO: Add Description** Optional.|
|portalLink|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [managementTemplateStep](../resources/managedtenants-managementtemplatestep.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_managementtemplatestep_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplateSteps
Content-Type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStep",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "category": "String",
  "provider": "String",
  "managementPortal": "String",
  "portalLink": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateStep"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateStep",
  "id": "118d7246-7246-118d-4672-8d1146728d11",
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "category": "String",
  "provider": "String",
  "managementPortal": "String",
  "portalLink": "String"
}
```

