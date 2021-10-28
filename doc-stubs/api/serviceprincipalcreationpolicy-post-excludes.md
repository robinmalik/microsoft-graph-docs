---
title: "Create servicePrincipalCreationConditionSet"
description: "Create a new servicePrincipalCreationConditionSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create servicePrincipalCreationConditionSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new servicePrincipalCreationConditionSet object.

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
POST /servicePrincipalCreationPolicy/excludes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object.

You can specify the following properties when creating a **servicePrincipalCreationConditionSet**.

|Property|Type|Description|
|:---|:---|:---|
|applicationIds|String collection|**TODO: Add Description** Optional.|
|applicationTenantIds|String collection|**TODO: Add Description** Optional.|
|applicationPublisherIds|String collection|**TODO: Add Description** Optional.|
|applicationsFromVerifiedPublisherOnly|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipalcreationconditionset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipalCreationPolicy/excludes
Content-Type: application/json
Content-length: 289

{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipalCreationConditionSet",
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
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.servicePrincipalCreationConditionSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipalCreationConditionSet",
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

