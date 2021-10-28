---
title: "Update servicePrincipalCreationConditionSet"
description: "Update the properties of a servicePrincipalCreationConditionSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update servicePrincipalCreationConditionSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object.

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
PATCH /servicePrincipalCreationPolicy/includes/{servicePrincipalCreationConditionSetId}
PATCH /servicePrincipalCreationPolicy/excludes/{servicePrincipalCreationConditionSetId}
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
|applicationIds|String collection|**TODO: Add Description** Optional.|
|applicationTenantIds|String collection|**TODO: Add Description** Optional.|
|applicationPublisherIds|String collection|**TODO: Add Description** Optional.|
|applicationsFromVerifiedPublisherOnly|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipalcreationconditionset"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/servicePrincipalCreationPolicy/includes/{servicePrincipalCreationConditionSetId}
Content-Type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.servicePrincipalCreationConditionSet",
  "applicationIds": [
    "String"
  ],
  "applicationTenantIds": [
    "String"
  ],
  "applicationPublisherIds": [
    "String"
  ],
  "applicationsFromVerifiedPublisherOnly": "Boolean"
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
  "@odata.type": "#microsoft.graph.servicePrincipalCreationConditionSet",
  "id": "666e960c-960c-666e-0c96-6e660c966e66",
  "applicationIds": [
    "String"
  ],
  "applicationTenantIds": [
    "String"
  ],
  "applicationPublisherIds": [
    "String"
  ],
  "applicationsFromVerifiedPublisherOnly": "Boolean"
}
```

