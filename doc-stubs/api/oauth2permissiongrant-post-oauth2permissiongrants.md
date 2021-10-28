---
title: "Create oAuth2PermissionGrant"
description: "Create a new oAuth2PermissionGrant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create oAuth2PermissionGrant
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
POST /oauth2PermissionGrants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

You can specify the following properties when creating an **oAuth2PermissionGrant**.

|Property|Type|Description|
|:---|:---|:---|
|clientId|String|**TODO: Add Description** Required.|
|consentType|String|**TODO: Add Description** Optional.|
|expiryTime|DateTimeOffset|**TODO: Add Description** Optional.|
|principalId|String|**TODO: Add Description** Optional.|
|resourceId|String|**TODO: Add Description** Required.|
|scope|String|**TODO: Add Description** Optional.|
|startTime|DateTimeOffset|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_oauth2permissiongrant_from_oauth2permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json
Content-length: 282

{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.oAuth2PermissionGrant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.oAuth2PermissionGrant",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "id": "3febe557-e557-3feb-57e5-eb3f57e5eb3f",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```

