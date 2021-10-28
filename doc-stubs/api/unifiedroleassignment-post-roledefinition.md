---
title: "Add unifiedRoleDefinition"
description: "Add roleDefinition by posting to the roleDefinition collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add unifiedRoleDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add roleDefinition by posting to the roleDefinition collection.

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
POST /groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/roleDefinition/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

You can specify the following properties when creating an **unifiedRoleDefinition**.

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

If successful, this method returns a `204 No Content` response code and an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/roleDefinition/$ref
Content-Type: application/json
Content-length: 385

{
  "@odata.type": "#Microsoft.DirectoryServices.unifiedRoleDefinition",
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
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.unifiedRoleDefinition"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.unifiedRoleDefinition",
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

