---
title: "accessPackageCatalog resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageCatalog resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageCatalogs](../api/accesspackagecatalog-list.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|Get a list of the [accessPackageCatalog](../resources/accesspackagecatalog.md) objects and their properties.|
|[Create accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Read the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Update accessPackageCatalog](../api/accesspackagecatalog-update.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Update the properties of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Delete accessPackageCatalog](../api/accesspackagecatalog-delete.md)|None|Deletes an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[List accessPackages](../api/accesspackagecatalog-list-accesspackages.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackage resources from the accessPackages navigation property.|
|[Create accessPackage](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Create a new accessPackage object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogType|accessPackageCatalogType|**TODO: Add Description**. The possible values are: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isExternallyVisible|Boolean|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|state|accessPackageCatalogState|**TODO: Add Description**. The possible values are: `unpublished`, `published`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackages|[accessPackage](../resources/accesspackage.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```

