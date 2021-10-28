---
title: "Update orgContact"
description: "Update the properties of an orgContact object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update orgContact
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [orgContact](../resources/orgcontact.md) object.

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
PATCH /contacts/{contactsId}
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
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|addresses|[Microsoft.DirectoryServices.physicalOfficeAddress](../resources/physicalofficeaddress.md) collection|**TODO: Add Description** Optional.|
|companyName|String|**TODO: Add Description** Optional.|
|department|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|givenName|String|**TODO: Add Description** Optional.|
|jobTitle|String|**TODO: Add Description** Optional.|
|mail|String|**TODO: Add Description** Optional.|
|mailNickname|String|**TODO: Add Description** Optional.|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description** Optional.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|onPremisesProvisioningErrors|[Microsoft.DirectoryServices.onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description** Optional.|
|phones|[Microsoft.DirectoryServices.phone](../resources/phone.md) collection|**TODO: Add Description** Optional.|
|proxyAddresses|String collection|**TODO: Add Description** Required.|
|surname|String|**TODO: Add Description** Optional.|
|cloudMSRtcIsSipEnabled|Boolean|**TODO: Add Description** Optional.|
|cloudMSRtcOwnerUrn|String|**TODO: Add Description** Optional.|
|cloudMSRtcPolicyAssignments|String collection|**TODO: Add Description** Optional.|
|cloudMSRtcPool|String|**TODO: Add Description** Optional.|
|cloudMSRtcServiceAttribute|[Microsoft.DirectoryServices.cloudMSRtcServiceAttributes](../resources/cloudmsrtcserviceattributes.md)|**TODO: Add Description** Optional.|
|cloudSipLine|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [orgContact](../resources/orgcontact.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/contacts/{contactsId}
Content-Type: application/json
Content-length: 1045

{
  "@odata.type": "#microsoft.graph.orgContact",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String",
  "cloudMSRtcIsSipEnabled": "Boolean",
  "cloudMSRtcOwnerUrn": "String",
  "cloudMSRtcPolicyAssignments": [
    "String"
  ],
  "cloudMSRtcPool": "String",
  "cloudMSRtcServiceAttribute": {
    "@odata.type": "microsoft.graph.cloudMSRtcServiceAttributes"
  },
  "cloudSipLine": "String"
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
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "a1d3e870-e870-a1d3-70e8-d3a170e8d3a1",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String",
  "cloudMSRtcIsSipEnabled": "Boolean",
  "cloudMSRtcOwnerUrn": "String",
  "cloudMSRtcPolicyAssignments": [
    "String"
  ],
  "cloudMSRtcPool": "String",
  "cloudMSRtcServiceAttribute": {
    "@odata.type": "microsoft.graph.cloudMSRtcServiceAttributes"
  },
  "cloudSipLine": "String"
}
```

