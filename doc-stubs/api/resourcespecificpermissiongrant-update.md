---
title: "Update resourceSpecificPermissionGrant"
description: "Update the properties of a resourceSpecificPermissionGrant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update resourceSpecificPermissionGrant
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

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
PATCH /permissionGrants/{permissionGrantsId}
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
|clientId|String|**TODO: Add Description** Optional.|
|clientAppId|String|**TODO: Add Description** Optional.|
|resourceAppId|String|**TODO: Add Description** Optional.|
|permissionType|String|**TODO: Add Description** Optional.|
|permission|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_resourcespecificpermissiongrant"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/permissionGrants/{permissionGrantsId}
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
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
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "2d6d0be5-0be5-2d6d-e50b-6d2de50b6d2d",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```

