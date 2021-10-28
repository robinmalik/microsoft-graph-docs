---
title: "Update endpoint"
description: "Update the properties of an endpoint object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update endpoint
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [endpoint](../resources/endpoint.md) object.

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
PATCH /groups/{groupsId}/endpoints/{endpointId}
PATCH /servicePrincipals/{servicePrincipalsId}/endpoints/{endpointId}
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
|capability|String|**TODO: Add Description** Required.|
|providerId|String|**TODO: Add Description** Optional.|
|providerName|String|**TODO: Add Description** Optional.|
|uri|String|**TODO: Add Description** Required.|
|providerResourceId|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_endpoint"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/endpoints/{endpointId}
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.endpoint",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
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
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "850ee2ba-e2ba-850e-bae2-0e85bae20e85",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```

