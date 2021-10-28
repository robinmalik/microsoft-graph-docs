---
title: "Create identityProviderBase"
description: "Create a new identityProviderBase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create identityProviderBase
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [identityProviderBase](../resources/identityproviderbase.md) object.

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
POST /directory/federationConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [identityProviderBase](../resources/identityproviderbase.md) object.

You can specify the following properties when creating an **identityProviderBase**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [identityProviderBase](../resources/identityproviderbase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identityproviderbase_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/federationConfigurations
Content-Type: application/json
Content-length: 102

{
  "@odata.type": "#Microsoft.DirectoryServices.identityProviderBase",
  "displayName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.identityProviderBase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.identityProviderBase",
  "id": "ae4a8fa5-8fa5-ae4a-a58f-4aaea58f4aae",
  "displayName": "String"
}
```

