---
title: "federatedIdentityCredential resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# federatedIdentityCredential resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List federatedIdentityCredentials](../api/federatedidentitycredential-list.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md) collection|Get a list of the [federatedIdentityCredential](../resources/federatedidentitycredential.md) objects and their properties.|
|[Create federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Create a new [federatedIdentityCredential](../resources/federatedidentitycredential.md) object.|
|[Get federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Read the properties and relationships of a [federatedIdentityCredential](../resources/federatedidentitycredential.md) object.|
|[Update federatedIdentityCredential](../api/federatedidentitycredential-update.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Update the properties of a [federatedIdentityCredential](../resources/federatedidentitycredential.md) object.|
|[Delete federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|None|Deletes a [federatedIdentityCredential](../resources/federatedidentitycredential.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audiences|String collection|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|issuer|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.federatedIdentityCredential",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```

