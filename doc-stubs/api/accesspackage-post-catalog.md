---
title: "Add accessPackageCatalog"
description: "Add catalog by posting to the catalog collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add accessPackageCatalog
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add catalog by posting to the catalog collection.

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
POST /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/catalog/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

You can specify the following properties when creating an **accessPackageCatalog**.

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|catalogType|accessPackageCatalogType|**TODO: Add Description**. The possible values are: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`. Optional.|
|state|accessPackageCatalogState|**TODO: Add Description**. The possible values are: `unpublished`, `published`, `unknownFutureValue`. Optional.|
|isExternallyVisible|Boolean|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `204 No Content` response code and an [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/catalog/$ref
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageCatalog",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageCatalog"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#Microsoft.IGAELM.EC.FrontEnd.ExternalModel.accessPackageCatalog",
  "id": "ef8826b4-26b4-ef88-b426-88efb42688ef",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```

