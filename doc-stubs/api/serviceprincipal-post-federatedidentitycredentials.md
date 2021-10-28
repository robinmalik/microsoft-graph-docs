---
title: "Create federatedIdentityCredential"
description: "Create a new federatedIdentityCredential object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create federatedIdentityCredential
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new federatedIdentityCredential object.

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
POST /servicePrincipals/{servicePrincipalsId}/federatedIdentityCredentials
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [federatedIdentityCredential](../resources/federatedidentitycredential.md) object.

You can specify the following properties when creating a **federatedIdentityCredential**.

|Property|Type|Description|
|:---|:---|:---|
|name|String|**TODO: Add Description** Required.|
|issuer|String|**TODO: Add Description** Required.|
|subject|String|**TODO: Add Description** Required.|
|description|String|**TODO: Add Description** Optional.|
|audiences|String collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and a [federatedIdentityCredential](../resources/federatedidentitycredential.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_federatedidentitycredential_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/federatedIdentityCredentials
Content-Type: application/json
Content-length: 215

{
  "@odata.type": "#Microsoft.DirectoryServices.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.federatedIdentityCredential"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```

