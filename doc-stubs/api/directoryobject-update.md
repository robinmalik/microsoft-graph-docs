---
title: "Update directoryObject"
description: "Update the properties of a directoryObject object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryObject
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [directoryObject](../resources/directoryobject.md) object.

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
PATCH /me/manager
PATCH /users/{usersId}/manager
PATCH /contacts/{contactsId}/manager
PATCH /me/memberOf/{directoryObjectId}
PATCH /groups/{groupsId}/createdOnBehalfOf
PATCH /me/ownedDevices/{directoryObjectId}
PATCH /me/ownedObjects/{directoryObjectId}
PATCH /me/directReports/{directoryObjectId}
PATCH /directoryObjects/{directoryObjectsId}
PATCH /me/createdObjects/{directoryObjectId}
PATCH /stsPolicy/appliesTo/{directoryObjectId}
PATCH /me/transitiveReports/{directoryObjectId}
PATCH /me/registeredDevices/{directoryObjectId}
PATCH /me/transitiveMemberOf/{directoryObjectId}
PATCH /directory/deletedItems/{directoryObjectId}
PATCH /applications/{applicationsId}/createdOnBehalfOf
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
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [directoryObject](../resources/directoryobject.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryobject"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/manager
Content-Type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.directoryObject",
  "deletedDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.directoryObject",
  "id": "ac8737f8-37f8-ac87-f837-87acf83787ac",
  "deletedDateTime": "String (timestamp)"
}
```

