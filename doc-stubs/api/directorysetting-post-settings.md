---
title: "Create directorySetting"
description: "Create a new directorySetting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directorySetting
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [directorySetting](../resources/directorysetting.md) object.

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
POST /settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directorySetting](../resources/directorysetting.md) object.

You can specify the following properties when creating a **directorySetting**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|templateId|String|**TODO: Add Description** Optional.|
|values|[Microsoft.DirectoryServices.settingValue](../resources/settingvalue.md) collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and a [directorySetting](../resources/directorysetting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}
-->
``` http
POST https://graph.microsoft.com/beta/settings
Content-Type: application/json
Content-length: 213

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySetting",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.directorySetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySetting",
  "id": "043790b5-90b5-0437-b590-3704b5903704",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```

