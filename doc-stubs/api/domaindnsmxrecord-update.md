---
title: "Update domainDnsMxRecord"
description: "Update the properties of a domainDnsMxRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update domainDnsMxRecord
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.

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
PATCH /domainDnsMxRecord
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
|isOptional|Boolean|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md). Required.|
|label|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md). Required.|
|recordType|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md). Optional.|
|supportedService|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md). Required.|
|ttl|Int32|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md). Required.|
|mailExchange|String|**TODO: Add Description** Required.|
|preference|Int32|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_domaindnsmxrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domainDnsMxRecord
Content-Type: application/json
Content-length: 247

{
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "mailExchange": "String",
  "preference": "Integer"
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
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "id": "f9ac104f-104f-f9ac-4f10-acf94f10acf9",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "mailExchange": "String",
  "preference": "Integer"
}
```

