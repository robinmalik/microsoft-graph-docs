---
title: "Update administrativeUnit"
description: "Update the properties of an administrativeUnit object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update administrativeUnit
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.

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
PATCH /administrativeUnits/{administrativeUnitsId}
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
|displayName|String|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|isMemberManagementRestricted|Boolean|**TODO: Add Description** Optional.|
|membershipRule|String|**TODO: Add Description** Optional.|
|membershipType|String|**TODO: Add Description** Optional.|
|membershipRuleProcessingState|String|**TODO: Add Description** Optional.|
|visibility|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{administrativeUnitsId}
Content-Type: application/json
Content-length: 341

{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "isMemberManagementRestricted": "Boolean",
  "membershipRule": "String",
  "membershipType": "String",
  "membershipRuleProcessingState": "String",
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
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "60973a94-3a94-6097-943a-9760943a9760",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "isMemberManagementRestricted": "Boolean",
  "membershipRule": "String",
  "membershipType": "String",
  "membershipRuleProcessingState": "String",
  "visibility": "String"
}
```

