---
title: "Update defaultUserRoleOverride"
description: "Update the properties of a defaultUserRoleOverride object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update defaultUserRoleOverride
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [defaultUserRoleOverride](../resources/defaultuserroleoverride.md) object.

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
PATCH /authorizationPolicy/defaultUserRoleOverrides/{defaultUserRoleOverrideId}
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
|isDefault|Boolean|**TODO: Add Description** Optional.|
|rolePermissions|[Microsoft.DirectoryServices.unifiedRolePermission](../resources/unifiedrolepermission.md) collection|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [defaultUserRoleOverride](../resources/defaultuserroleoverride.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_defaultuserroleoverride"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authorizationPolicy/defaultUserRoleOverrides/{defaultUserRoleOverrideId}
Content-Type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.defaultUserRoleOverride",
  "isDefault": "Boolean",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ]
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
  "@odata.type": "#microsoft.graph.defaultUserRoleOverride",
  "id": "5262052e-052e-5262-2e05-62522e056252",
  "isDefault": "Boolean",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ]
}
```

