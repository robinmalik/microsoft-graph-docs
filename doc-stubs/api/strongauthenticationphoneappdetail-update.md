---
title: "Update strongAuthenticationPhoneAppDetail"
description: "Update the properties of a strongAuthenticationPhoneAppDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update strongAuthenticationPhoneAppDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.

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
PATCH /me/strongAuthenticationDetail/phoneAppDetails/{strongAuthenticationPhoneAppDetailId}
PATCH /users/{usersId}/strongAuthenticationDetail/phoneAppDetails/{strongAuthenticationPhoneAppDetailId}
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

If successful, this method returns a `200 OK` response code and an updated [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_strongauthenticationphoneappdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/strongAuthenticationDetail/phoneAppDetails/{strongAuthenticationPhoneAppDetailId}
Content-Type: application/json
Content-length: 643

{
  "@odata.type": "#microsoft.graph.strongAuthenticationPhoneAppDetail",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.strongAuthenticationPhoneAppDetail",
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

