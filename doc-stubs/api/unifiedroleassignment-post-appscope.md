---
title: "Create appScope"
description: "Create a new appScope object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create appScope
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [appScope](../resources/appscope.md) object.

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
POST ** Collection URI for Microsoft.DirectoryServices.appScope not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [appScope](../resources/appscope.md) object.

You can specify the following properties when creating an **appScope**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|type|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [appScope](../resources/appscope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_appscope_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.appScope not found
Content-Type: application/json
Content-length: 111

{
  "@odata.type": "#Microsoft.DirectoryServices.appScope",
  "displayName": "String",
  "type": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.appScope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.appScope",
  "id": "f44f0aed-0aed-f44f-ed0a-4ff4ed0a4ff4",
  "displayName": "String",
  "type": "String"
}
```

