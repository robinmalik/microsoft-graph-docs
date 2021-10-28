---
title: "Create strongAuthenticationPhoneAppDetail"
description: "Create a new strongAuthenticationPhoneAppDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create strongAuthenticationPhoneAppDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.

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
POST /me/strongAuthenticationDetail/phoneAppDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.

You can specify the following properties when creating a **strongAuthenticationPhoneAppDetail**.

|Property|Type|Description|
|:---|:---|:---|
|authenticatorFlavor|String|**TODO: Add Description** Optional.|
|authenticationType|String|**TODO: Add Description** Required.|
|deviceId|Guid|**TODO: Add Description** Optional.|
|deviceToken|String|**TODO: Add Description** Optional.|
|deviceName|String|**TODO: Add Description** Optional.|
|deviceTag|String|**TODO: Add Description** Optional.|
|hashFunction|String|**TODO: Add Description** Optional.|
|lastAuthenticatedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|oathTokenMetadata|[Microsoft.DirectoryServices.oathTokenMetadata](../resources/oathtokenmetadata.md)|**TODO: Add Description** Optional.|
|oathSecretKey|String|**TODO: Add Description** Optional.|
|oathTokenTimeDriftInSeconds|Int32|**TODO: Add Description** Required.|
|tenantDeviceId|String|**TODO: Add Description** Optional.|
|tokenGenerationIntervalInSeconds|Int32|**TODO: Add Description** Optional.|
|phoneAppVersion|String|**TODO: Add Description** Optional.|
|notificationType|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_strongauthenticationphoneappdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/strongAuthenticationDetail/phoneAppDetails
Content-Type: application/json
Content-length: 655

{
  "@odata.type": "#Microsoft.DirectoryServices.strongAuthenticationPhoneAppDetail",
  "authenticatorFlavor": "String",
  "authenticationType": "String",
  "deviceId": "Guid",
  "deviceToken": "String",
  "deviceName": "String",
  "deviceTag": "String",
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
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.strongAuthenticationPhoneAppDetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```

