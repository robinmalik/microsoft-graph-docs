---
title: "Update identityProviderBase"
description: "Update the properties of an identityProviderBase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update identityProviderBase
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [identityProviderBase](../resources/identityproviderbase.md) object.

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
PATCH /directory/federationConfigurations/{identityProviderBaseId}
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
|displayName|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [identityProviderBase](../resources/identityproviderbase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_identityproviderbase"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/federationConfigurations/{identityProviderBaseId}
Content-Type: application/json
Content-length: 90

{
  "@odata.type": "#microsoft.graph.identityProviderBase",
  "displayName": "String"
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
  "@odata.type": "#microsoft.graph.identityProviderBase",
  "id": "ae4a8fa5-8fa5-ae4a-a58f-4aaea58f4aae",
  "displayName": "String"
}
```

