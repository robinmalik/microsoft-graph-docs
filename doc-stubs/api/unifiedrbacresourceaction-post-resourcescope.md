---
title: "Create unifiedRbacResourceScope"
description: "Create a new unifiedRbacResourceScope object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create unifiedRbacResourceScope
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) object.

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
POST ** Collection URI for Microsoft.DirectoryServices.unifiedRbacResourceScope not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) object.

You can specify the following properties when creating an **unifiedRbacResourceScope**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|scope|String|**TODO: Add Description** Required.|
|type|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_unifiedrbacresourcescope_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.unifiedRbacResourceScope not found
Content-Type: application/json
Content-length: 149

{
  "@odata.type": "#Microsoft.DirectoryServices.unifiedRbacResourceScope",
  "displayName": "String",
  "scope": "String",
  "type": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.unifiedRbacResourceScope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.unifiedRbacResourceScope",
  "id": "e0c7c65b-c65b-e0c7-5bc6-c7e05bc6c7e0",
  "displayName": "String",
  "scope": "String",
  "type": "String"
}
```

