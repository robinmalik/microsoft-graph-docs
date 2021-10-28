---
title: "Create domain"
description: "Create a new domain object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create domain
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [domain](../resources/domain.md) object.

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
POST /domains
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [domain](../resources/domain.md) object.

You can specify the following properties when creating a **domain**.

|Property|Type|Description|
|:---|:---|:---|
|authenticationType|String|**TODO: Add Description** Required.|
|availabilityStatus|String|**TODO: Add Description** Optional.|
|isAdminManaged|Boolean|**TODO: Add Description** Required.|
|isDefault|Boolean|**TODO: Add Description** Required.|
|isInitial|Boolean|**TODO: Add Description** Required.|
|isRoot|Boolean|**TODO: Add Description** Required.|
|isVerified|Boolean|**TODO: Add Description** Required.|
|passwordNotificationWindowInDays|Int32|**TODO: Add Description** Optional.|
|passwordValidityPeriodInDays|Int32|**TODO: Add Description** Optional.|
|supportedServices|String collection|**TODO: Add Description** Required.|
|state|[Microsoft.DirectoryServices.domainState](../resources/domainstate.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [domain](../resources/domain.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_domain_from_domains"
}
-->
``` http
POST https://graph.microsoft.com/beta/domains
Content-Type: application/json
Content-length: 480

{
  "@odata.type": "#Microsoft.DirectoryServices.domain",
  "authenticationType": "String",
  "availabilityStatus": "String",
  "isAdminManaged": "Boolean",
  "isDefault": "Boolean",
  "isInitial": "Boolean",
  "isRoot": "Boolean",
  "isVerified": "Boolean",
  "passwordNotificationWindowInDays": "Integer",
  "passwordValidityPeriodInDays": "Integer",
  "supportedServices": [
    "String"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.domain"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.domain",
  "authenticationType": "String",
  "availabilityStatus": "String",
  "isAdminManaged": "Boolean",
  "isDefault": "Boolean",
  "isInitial": "Boolean",
  "isRoot": "Boolean",
  "isVerified": "Boolean",
  "id": "9162c656-c656-9162-56c6-629156c66291",
  "passwordNotificationWindowInDays": "Integer",
  "passwordValidityPeriodInDays": "Integer",
  "supportedServices": [
    "String"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState"
  }
}
```

