---
title: "List accessPackageSubjects"
description: "Get a list of the accessPackageSubject objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageSubjects
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [accessPackageSubject](../resources/accesspackagesubject.md) objects and their properties.

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
GET ** Collection URI for Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageSubject not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [accessPackageSubject](../resources/accesspackagesubject.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_accesspackagesubject"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageSubject not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageSubject)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageSubject",
      "id": "913ad345-d345-913a-45d3-3a9145d33a91",
      "objectId": "String",
      "displayName": "String",
      "principalName": "String",
      "email": "String",
      "onPremisesSecurityIdentifier": "String",
      "subjectType": "String"
    }
  ]
}
```

