---
title: "Update unifiedRoleDefinition"
description: "Update the properties of an unifiedRoleDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRoleDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

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
PATCH /groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/roleDefinition
PATCH /groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/roleDefinition/inheritsPermissionsFrom/{unifiedRoleDefinitionId}
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
|description|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|isBuiltIn|Boolean|**TODO: Add Description** Optional.|
|isEnabled|Boolean|**TODO: Add Description** Optional.|
|resourceScopes|String collection|**TODO: Add Description** Required.|
|rolePermissions|[Microsoft.DirectoryServices.unifiedRolePermission](../resources/unifiedrolepermission.md) collection|**TODO: Add Description** Required.|
|templateId|String|**TODO: Add Description** Optional.|
|version|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/roleDefinition
Content-Type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "description": "String",
  "displayName": "String",
  "isBuiltIn": "Boolean",
  "isEnabled": "Boolean",
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
  "templateId": "String",
  "version": "String"
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
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "description": "String",
  "displayName": "String",
  "id": "0359e67b-e67b-0359-7be6-59037be65903",
  "isBuiltIn": "Boolean",
  "isEnabled": "Boolean",
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
  "templateId": "String",
  "version": "String"
}
```

