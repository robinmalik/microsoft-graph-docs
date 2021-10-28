---
title: "Update permissionGrantConditionSet"
description: "Update the properties of a permissionGrantConditionSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update permissionGrantConditionSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.

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
PATCH /permissionGrantPolicy/includes/{permissionGrantConditionSetId}
PATCH /permissionGrantPolicy/excludes/{permissionGrantConditionSetId}
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
|permissionClassification|String|**TODO: Add Description** Optional.|
|permissionType|permissionType|**TODO: Add Description**. The possible values are: `application`, `delegated`, `delegatedUserConsentable`. Optional.|
|resourceApplication|String|**TODO: Add Description** Optional.|
|permissions|String collection|**TODO: Add Description** Optional.|
|clientApplicationIds|String collection|**TODO: Add Description** Optional.|
|clientApplicationTenantIds|String collection|**TODO: Add Description** Optional.|
|clientApplicationPublisherIds|String collection|**TODO: Add Description** Optional.|
|clientApplicationsFromVerifiedPublisherOnly|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantconditionset"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/permissionGrantPolicy/includes/{permissionGrantConditionSetId}
Content-Type: application/json
Content-length: 440

{
  "@odata.type": "#microsoft.graph.permissionGrantConditionSet",
  "permissionClassification": "String",
  "permissionType": "String",
  "resourceApplication": "String",
  "permissions": [
    "String"
  ],
  "clientApplicationIds": [
    "String"
  ],
  "clientApplicationTenantIds": [
    "String"
  ],
  "clientApplicationPublisherIds": [
    "String"
  ],
  "clientApplicationsFromVerifiedPublisherOnly": "Boolean"
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
  "@odata.type": "#microsoft.graph.permissionGrantConditionSet",
  "id": "00e3a9a6-a9a6-00e3-a6a9-e300a6a9e300",
  "permissionClassification": "String",
  "permissionType": "String",
  "resourceApplication": "String",
  "permissions": [
    "String"
  ],
  "clientApplicationIds": [
    "String"
  ],
  "clientApplicationTenantIds": [
    "String"
  ],
  "clientApplicationPublisherIds": [
    "String"
  ],
  "clientApplicationsFromVerifiedPublisherOnly": "Boolean"
}
```

