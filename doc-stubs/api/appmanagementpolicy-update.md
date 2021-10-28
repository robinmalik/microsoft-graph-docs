---
title: "Update appManagementPolicy"
description: "Update the properties of an appManagementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update appManagementPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [appManagementPolicy](../resources/appmanagementpolicy.md) object.

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
PATCH /policyRoot/appManagementPolicies/{appManagementPolicyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|isEnabled|Boolean|**TODO: Add Description** Required.|
|restrictions|[Microsoft.DirectoryServices.appManagementConfiguration](../resources/appmanagementconfiguration.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [appManagementPolicy](../resources/appmanagementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_appmanagementpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policyRoot/appManagementPolicies/{appManagementPolicyId}
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.appManagementPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "restrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.appManagementPolicy",
  "id": "fbfa322e-322e-fbfa-2e32-fafb2e32fafb",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "restrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```

