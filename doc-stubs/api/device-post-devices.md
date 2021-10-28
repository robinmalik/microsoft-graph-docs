---
title: "Create device"
description: "Create a new device object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create device
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [device](../resources/device.md) object.

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
POST /devices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [device](../resources/device.md) object.

You can specify the following properties when creating a **device**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|accountEnabled|Boolean|**TODO: Add Description** Optional.|
|alternativeSecurityIds|[Microsoft.DirectoryServices.alternativeSecurityId](../resources/alternativesecurityid.md) collection|**TODO: Add Description** Required.|
|approximateLastSignInDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|complianceExpirationDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|customSecurityAttributes|[Microsoft.DirectoryServices.customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|**TODO: Add Description** Optional.|
|deviceCategory|String|**TODO: Add Description** Optional.|
|deviceId|String|**TODO: Add Description** Optional.|
|deviceMetadata|String|**TODO: Add Description** Optional.|
|deviceOwnership|String|**TODO: Add Description** Optional.|
|deviceVersion|Int32|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|domainName|String|**TODO: Add Description** Optional.|
|enrollmentProfileName|String|**TODO: Add Description** Optional.|
|enrollmentType|String|**TODO: Add Description** Optional.|
|extensionAttributes|[Microsoft.DirectoryServices.onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description** Optional.|
|isCompliant|Boolean|**TODO: Add Description** Optional.|
|isManaged|Boolean|**TODO: Add Description** Optional.|
|isManagementRestricted|Boolean|**TODO: Add Description** Optional.|
|isRooted|Boolean|**TODO: Add Description** Optional.|
|managementType|String|**TODO: Add Description** Optional.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description** Optional.|
|operatingSystem|String|**TODO: Add Description** Optional.|
|operatingSystemVersion|String|**TODO: Add Description** Optional.|
|hostnames|String collection|**TODO: Add Description** Optional.|
|physicalIds|String collection|**TODO: Add Description** Required.|
|profileType|String|**TODO: Add Description** Optional.|
|registrationDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|systemLabels|String collection|**TODO: Add Description** Required.|
|trustType|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [device](../resources/device.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}
-->
``` http
POST https://graph.microsoft.com/beta/devices
Content-Type: application/json
Content-length: 1386

{
  "@odata.type": "#Microsoft.DirectoryServices.device",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": "Boolean",
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId"
    }
  ],
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "deviceCategory": "String",
  "deviceId": "String",
  "deviceMetadata": "String",
  "deviceOwnership": "String",
  "deviceVersion": "Integer",
  "displayName": "String",
  "domainName": "String",
  "enrollmentProfileName": "String",
  "enrollmentType": "String",
  "extensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "isCompliant": "Boolean",
  "isManaged": "Boolean",
  "isManagementRestricted": "Boolean",
  "isRooted": "Boolean",
  "managementType": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "operatingSystem": "String",
  "operatingSystemVersion": "String",
  "hostnames": [
    "String"
  ],
  "physicalIds": [
    "String"
  ],
  "profileType": "String",
  "registrationDateTime": "String (timestamp)",
  "systemLabels": [
    "String"
  ],
  "trustType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.device"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.device",
  "id": "0fa4299e-299e-0fa4-9e29-a40f9e29a40f",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": "Boolean",
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId"
    }
  ],
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "deviceCategory": "String",
  "deviceId": "String",
  "deviceMetadata": "String",
  "deviceOwnership": "String",
  "deviceVersion": "Integer",
  "displayName": "String",
  "domainName": "String",
  "enrollmentProfileName": "String",
  "enrollmentType": "String",
  "extensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "isCompliant": "Boolean",
  "isManaged": "Boolean",
  "isManagementRestricted": "Boolean",
  "isRooted": "Boolean",
  "managementType": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "operatingSystem": "String",
  "operatingSystemVersion": "String",
  "hostnames": [
    "String"
  ],
  "physicalIds": [
    "String"
  ],
  "profileType": "String",
  "registrationDateTime": "String (timestamp)",
  "systemLabels": [
    "String"
  ],
  "trustType": "String"
}
```

