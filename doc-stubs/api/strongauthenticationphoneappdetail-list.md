---
title: "List strongAuthenticationPhoneAppDetails"
description: "Get a list of the strongAuthenticationPhoneAppDetail objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List strongAuthenticationPhoneAppDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) objects and their properties.

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
GET /me/strongAuthenticationDetail/phoneAppDetails
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_strongauthenticationphoneappdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/strongAuthenticationDetail/phoneAppDetails
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.strongAuthenticationPhoneAppDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.strongAuthenticationPhoneAppDetail",
      "authenticatorFlavor": "String",
      "authenticationType": "String",
      "deviceId": "Guid",
      "deviceToken": "String",
      "deviceName": "String",
      "deviceTag": "String",
      "id": "24a8b0c7-b0c7-24a8-c7b0-a824c7b0a824",
      "hashFunction": "String",
      "lastAuthenticatedDateTime": "String (timestamp)",
      "oathTokenMetadata": {
        "@odata.type": "microsoft.graph.oathTokenMetadata"
      },
      "oathSecretKey": "String",
      "oathTokenTimeDriftInSeconds": "Integer",
      "tenantDeviceId": "String",
      "tokenGenerationIntervalInSeconds": "Integer",
      "phoneAppVersion": "String",
      "notificationType": "String"
    }
  ]
}
```

