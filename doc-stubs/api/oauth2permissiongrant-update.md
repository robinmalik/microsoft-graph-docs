---
title: "Update oAuth2PermissionGrant"
description: "Update the properties of an oAuth2PermissionGrant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update oAuth2PermissionGrant
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.

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
PATCH /oauth2PermissionGrants/{oauth2PermissionGrantsId}
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
|clientId|String|**TODO: Add Description** Required.|
|consentType|String|**TODO: Add Description** Optional.|
|expiryTime|DateTimeOffset|**TODO: Add Description** Optional.|
|principalId|String|**TODO: Add Description** Optional.|
|resourceId|String|**TODO: Add Description** Required.|
|scope|String|**TODO: Add Description** Optional.|
|startTime|DateTimeOffset|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_oauth2permissiongrant"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/oauth2PermissionGrants/{oauth2PermissionGrantsId}
Content-Type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
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

