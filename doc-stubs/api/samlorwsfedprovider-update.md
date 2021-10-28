---
title: "Update samlOrWsFedProvider"
description: "Update the properties of a samlOrWsFedProvider object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update samlOrWsFedProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) object.

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
PATCH /samlOrWsFedProvider
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
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md). Optional.|
|issuerUri|String|**TODO: Add Description** Optional.|
|metadataExchangeUri|String|**TODO: Add Description** Optional.|
|signingCertificate|String|**TODO: Add Description** Optional.|
|passiveSignInUri|String|**TODO: Add Description** Optional.|
|preferredAuthenticationProtocol|authenticationProtocol|**TODO: Add Description**. The possible values are: `wsFed`, `saml`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_samlorwsfedprovider"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/samlOrWsFedProvider
Content-Type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
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
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "id": "f20d7ec2-7ec2-f20d-c27e-0df2c27e0df2",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```

