---
title: "strongAuthenticationPhoneAppDetail resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# strongAuthenticationPhoneAppDetail resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List strongAuthenticationPhoneAppDetails](../api/strongauthenticationphoneappdetail-list.md)|[strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) collection|Get a list of the [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) objects and their properties.|
|[Create strongAuthenticationPhoneAppDetail](../api/strongauthenticationdetail-post-phoneappdetails.md)|[strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md)|Create a new [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.|
|[Get strongAuthenticationPhoneAppDetail](../api/strongauthenticationphoneappdetail-get.md)|[strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md)|Read the properties and relationships of a [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.|
|[Update strongAuthenticationPhoneAppDetail](../api/strongauthenticationphoneappdetail-update.md)|[strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md)|Update the properties of a [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.|
|[Delete strongAuthenticationPhoneAppDetail](../api/strongauthenticationphoneappdetail-delete.md)|None|Deletes a [strongAuthenticationPhoneAppDetail](../resources/strongauthenticationphoneappdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationType|String|**TODO: Add Description**|
|authenticatorFlavor|String|**TODO: Add Description**|
|deviceId|Guid|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|deviceTag|String|**TODO: Add Description**|
|deviceToken|String|**TODO: Add Description**|
|hashFunction|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastAuthenticatedDateTime|DateTimeOffset|**TODO: Add Description**|
|notificationType|String|**TODO: Add Description**|
|oathSecretKey|String|**TODO: Add Description**|
|oathTokenMetadata|[oathTokenMetadata](../resources/oathtokenmetadata.md)|**TODO: Add Description**|
|oathTokenTimeDriftInSeconds|Int32|**TODO: Add Description**|
|phoneAppVersion|String|**TODO: Add Description**|
|tenantDeviceId|String|**TODO: Add Description**|
|tokenGenerationIntervalInSeconds|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.strongAuthenticationPhoneAppDetail",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.strongAuthenticationPhoneAppDetail",
  "authenticatorFlavor": "String",
  "authenticationType": "String",
  "deviceId": "Guid",
  "deviceToken": "String",
  "deviceName": "String",
  "deviceTag": "String",
  "id": "String (identifier)",
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

