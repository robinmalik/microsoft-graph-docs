---
title: "Create rbacApplication"
description: "Create a new rbacApplication object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create rbacApplication
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [rbacApplication](../resources/rbacapplication.md) object.

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
POST ** Collection URI for BadUnresolvedEntityType:Microsoft.IGAELM.EC.FrontEnd.ExternalModel.rbacApplication not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [rbacApplication](../resources/rbacapplication.md) object.

You can specify the following properties when creating a **rbacApplication**.

|Property|Type|Description|
|:---|:---|:---|



## Response

If successful, this method returns a `201 Created` response code and a [rbacApplication](../resources/rbacapplication.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_rbacapplication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for BadUnresolvedEntityType:Microsoft.IGAELM.EC.FrontEnd.ExternalModel.rbacApplication not found
Content-Type: application/json
Content-length: 84

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.rbacApplication"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.IGAELM.EC.FrontEnd.ExternalModel.rbacApplication"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.rbacApplication"
}
```

