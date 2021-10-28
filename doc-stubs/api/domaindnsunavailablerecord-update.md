---
title: "Update domainDnsUnavailableRecord"
description: "Update the properties of a domainDnsUnavailableRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update domainDnsUnavailableRecord
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.

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
PATCH /domainDnsUnavailableRecord
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
|description|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_domaindnsunavailablerecord"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domainDnsUnavailableRecord
Content-Type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "description": "String"
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
  "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
  "id": "1895b64b-b64b-1895-4bb6-95184bb69518",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "description": "String"
}
```

