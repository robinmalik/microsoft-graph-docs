---
title: "Update appScope"
description: "Update the properties of an appScope object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update appScope
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [appScope](../resources/appscope.md) object.

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
PATCH /groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/appScope
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
|displayName|String|**TODO: Add Description** Optional.|
|type|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [appScope](../resources/appscope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_appscope"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/roleManagement/directory/transitiveRoleAssignments/{unifiedRoleAssignmentId}/appScope
Content-Type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.appScope",
  "displayName": "String",
  "type": "String"
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
  "@odata.type": "#microsoft.graph.appScope",
  "id": "f44f0aed-0aed-f44f-ed0a-4ff4ed0a4ff4",
  "displayName": "String",
  "type": "String"
}
```

