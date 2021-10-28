---
title: "Create organization"
description: "Create a new organization object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create organization
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [organization](../resources/organization.md) object.

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
POST /organization
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [organization](../resources/organization.md) object.

You can specify the following properties when creating an **organization**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|assignedPlans|[Microsoft.DirectoryServices.assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description** Required.|
|businessPhones|String collection|**TODO: Add Description** Required.|
|city|String|**TODO: Add Description** Optional.|
|companyTags|String collection|**TODO: Add Description** Optional.|
|country|String|**TODO: Add Description** Optional.|
|countryLetterCode|String|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|dataBoundary|dataBoundary|**TODO: Add Description**. The possible values are: `none`, `eu`, `unknownFutureValue`. Required.|
|directorySizeQuota|[Microsoft.DirectoryServices.directorySizeQuota](../resources/directorysizequota.md)|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|isMultipleDataLocationsForServicesEnabled|Boolean|**TODO: Add Description** Optional.|
|licenseMigrationInfo|[Microsoft.DirectoryServices.licenseMigrationInfo](../resources/licensemigrationinfo.md)|**TODO: Add Description** Optional.|
|marketingNotificationEmails|String collection|**TODO: Add Description** Required.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description** Optional.|
|postalCode|String|**TODO: Add Description** Optional.|
|preferredLanguage|String|**TODO: Add Description** Optional.|
|privacyProfile|[Microsoft.DirectoryServices.privacyProfile](../resources/privacyprofile.md)|**TODO: Add Description** Optional.|
|provisionedPlans|[Microsoft.DirectoryServices.provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description** Required.|
|releaseTrack|String|**TODO: Add Description** Optional.|
|replicationScope|String|**TODO: Add Description** Required.|
|securityComplianceNotificationMails|String collection|**TODO: Add Description** Required.|
|securityComplianceNotificationPhones|String collection|**TODO: Add Description** Required.|
|state|String|**TODO: Add Description** Optional.|
|street|String|**TODO: Add Description** Optional.|
|technicalNotificationMails|String collection|**TODO: Add Description** Required.|
|verifiedDomains|[Microsoft.DirectoryServices.verifiedDomain](../resources/verifieddomain.md) collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and an [organization](../resources/organization.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organization_from_organization"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization
Content-Type: application/json
Content-length: 1451

{
  "@odata.type": "#Microsoft.DirectoryServices.organization",
  "deletedDateTime": "String (timestamp)",
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyTags": [
    "String"
  ],
  "country": "String",
  "countryLetterCode": "String",
  "dataBoundary": "String",
  "directorySizeQuota": {
    "@odata.type": "microsoft.graph.directorySizeQuota"
  },
  "displayName": "String",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "licenseMigrationInfo": {
    "@odata.type": "microsoft.graph.licenseMigrationInfo"
  },
  "marketingNotificationEmails": [
    "String"
  ],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "releaseTrack": "String",
  "replicationScope": "String",
  "securityComplianceNotificationMails": [
    "String"
  ],
  "securityComplianceNotificationPhones": [
    "String"
  ],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": [
    "String"
  ],
  "verifiedDomains": [
    {
      "@odata.type": "microsoft.graph.verifiedDomain"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.organization"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.organization",
  "id": "d8606e02-6e02-d860-026e-60d8026e60d8",
  "deletedDateTime": "String (timestamp)",
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyTags": [
    "String"
  ],
  "country": "String",
  "countryLetterCode": "String",
  "createdDateTime": "String (timestamp)",
  "dataBoundary": "String",
  "directorySizeQuota": {
    "@odata.type": "microsoft.graph.directorySizeQuota"
  },
  "displayName": "String",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "licenseMigrationInfo": {
    "@odata.type": "microsoft.graph.licenseMigrationInfo"
  },
  "marketingNotificationEmails": [
    "String"
  ],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": "Boolean",
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {
    "@odata.type": "microsoft.graph.privacyProfile"
  },
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "releaseTrack": "String",
  "replicationScope": "String",
  "securityComplianceNotificationMails": [
    "String"
  ],
  "securityComplianceNotificationPhones": [
    "String"
  ],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": [
    "String"
  ],
  "verifiedDomains": [
    {
      "@odata.type": "microsoft.graph.verifiedDomain"
    }
  ]
}
```

