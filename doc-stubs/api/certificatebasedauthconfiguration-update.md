---
title: "Update certificateBasedAuthConfiguration"
description: "Update the properties of a certificateBasedAuthConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update certificateBasedAuthConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.

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
PATCH /certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
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
|certificateAuthorities|[Microsoft.DirectoryServices.certificateAuthority](../resources/certificateauthority.md) collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `200 OK` response code and an updated [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_certificatebasedauthconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/certificateBasedAuthConfiguration/{certificateBasedAuthConfigurationId}
Content-Type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
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
  "@odata.type": "#microsoft.graph.certificateBasedAuthConfiguration",
  "id": "47407e10-7e10-4740-107e-4047107e4047",
  "certificateAuthorities": [
    {
      "@odata.type": "microsoft.graph.certificateAuthority"
    }
  ]
}
```

