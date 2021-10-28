---
title: "Create endpoint"
description: "Create a new endpoint object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create endpoint
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new endpoint object.

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
POST /servicePrincipals/{servicePrincipalsId}/endpoints
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [endpoint](../resources/endpoint.md) object.

You can specify the following properties when creating an **endpoint**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|capability|String|**TODO: Add Description** Required.|
|providerId|String|**TODO: Add Description** Optional.|
|providerName|String|**TODO: Add Description** Optional.|
|uri|String|**TODO: Add Description** Required.|
|providerResourceId|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [endpoint](../resources/endpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_endpoint_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/endpoints
Content-Type: application/json
Content-length: 244

{
  "@odata.type": "#Microsoft.DirectoryServices.endpoint",
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
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.endpoint"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.endpoint",
  "id": "850ee2ba-e2ba-850e-bae2-0e85bae20e85",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```

