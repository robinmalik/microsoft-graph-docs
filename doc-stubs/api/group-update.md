---
title: "Update group"
description: "Update the properties of a group object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update group
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [group](../resources/group.md) object.

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
PATCH /groups/{groupsId}
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
|assignedLabels|[Microsoft.DirectoryServices.assignedLabel](../resources/assignedlabel.md) collection|**TODO: Add Description** Optional.|
|assignedLicenses|[Microsoft.DirectoryServices.assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description** Optional.|
|classification|String|**TODO: Add Description** Optional.|
|createdByAppId|String|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|expirationDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|groupTypes|String collection|**TODO: Add Description** Required.|
|hasMembersWithLicenseErrors|Boolean|**TODO: Add Description** Optional.|
|infoCatalogs|String collection|**TODO: Add Description** Required.|
|isAssignableToRole|Boolean|**TODO: Add Description** Optional.|
|isManagementRestricted|Boolean|**TODO: Add Description** Optional.|
|licenseProcessingState|[Microsoft.DirectoryServices.licenseProcessingState](../resources/licenseprocessingstate.md)|**TODO: Add Description** Optional.|
|mail|String|**TODO: Add Description** Optional.|
|mailEnabled|Boolean|**TODO: Add Description** Optional.|
|mailNickname|String|**TODO: Add Description** Optional.|
|mdmAppId|String|**TODO: Add Description** Optional.|
|membershipRule|String|**TODO: Add Description** Optional.|
|membershipRuleProcessingState|String|**TODO: Add Description** Optional.|
|onPremisesDomainName|String|**TODO: Add Description** Optional.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|onPremisesNetBiosName|String|**TODO: Add Description** Optional.|
|onPremisesProvisioningErrors|[Microsoft.DirectoryServices.onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description** Optional.|
|onPremisesSamAccountName|String|**TODO: Add Description** Optional.|
|onPremisesSecurityIdentifier|String|**TODO: Add Description** Optional.|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description** Optional.|
|organizationId|String|**TODO: Add Description** Optional.|
|preferredDataLocation|String|**TODO: Add Description** Optional.|
|preferredLanguage|String|**TODO: Add Description** Optional.|
|proxyAddresses|String collection|**TODO: Add Description** Required.|
|renewedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|resourceBehaviorOptions|String collection|**TODO: Add Description** Required.|
|resourceProvisioningOptions|String collection|**TODO: Add Description** Required.|
|securityEnabled|Boolean|**TODO: Add Description** Optional.|
|securityIdentifier|String|**TODO: Add Description** Optional.|
|theme|String|**TODO: Add Description** Optional.|
|visibility|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [group](../resources/group.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_group"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}
Content-Type: application/json
Content-length: 1729

{
  "@odata.type": "#microsoft.graph.group",
  "deletedDateTime": "String (timestamp)",
  "assignedLabels": [
    {
      "@odata.type": "microsoft.graph.assignedLabel"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "classification": "String",
  "createdByAppId": "String",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": "Boolean",
  "infoCatalogs": [
    "String"
  ],
  "isAssignableToRole": "Boolean",
  "isManagementRestricted": "Boolean",
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState"
  },
  "mail": "String",
  "mailEnabled": "Boolean",
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "organizationId": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": [
    "String"
  ],
  "resourceProvisioningOptions": [
    "String"
  ],
  "securityEnabled": "Boolean",
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String"
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
  "@odata.type": "#microsoft.graph.group",
  "id": "ebb92376-2376-ebb9-7623-b9eb7623b9eb",
  "deletedDateTime": "String (timestamp)",
  "assignedLabels": [
    {
      "@odata.type": "microsoft.graph.assignedLabel"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "classification": "String",
  "createdByAppId": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": "Boolean",
  "infoCatalogs": [
    "String"
  ],
  "isAssignableToRole": "Boolean",
  "isManagementRestricted": "Boolean",
  "licenseProcessingState": {
    "@odata.type": "microsoft.graph.licenseProcessingState"
  },
  "mail": "String",
  "mailEnabled": "Boolean",
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "organizationId": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": [
    "String"
  ],
  "resourceProvisioningOptions": [
    "String"
  ],
  "securityEnabled": "Boolean",
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String"
}
```

