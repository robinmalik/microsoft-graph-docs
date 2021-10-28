---
title: "Create directorySettingTemplate"
description: "Create a new directorySettingTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directorySettingTemplate
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [directorySettingTemplate](../resources/directorysettingtemplate.md) object.

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
POST /directorySettingTemplates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directorySettingTemplate](../resources/directorysettingtemplate.md) object.

You can specify the following properties when creating a **directorySettingTemplate**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|values|[Microsoft.DirectoryServices.settingTemplateValue](../resources/settingtemplatevalue.md) collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and a [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorysettingtemplate_from_directorysettingtemplates"
}
-->
``` http
POST https://graph.microsoft.com/beta/directorySettingTemplates
Content-Type: application/json
Content-length: 274

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.directorySettingTemplate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
  "id": "e52fe0c9-e0c9-e52f-c9e0-2fe5c9e02fe5",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue"
    }
  ]
}
```

