---
title: "Create administrativeUnit"
description: "Create a new administrativeUnit object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create administrativeUnit
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new administrativeUnit object.

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
POST /directory/administrativeUnits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [administrativeUnit](../resources/administrativeunit.md) object.

You can specify the following properties when creating an **administrativeUnit**.

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

If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/administrativeUnits
Content-Type: application/json
Content-length: 353

{
  "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
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
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.administrativeUnit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
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

