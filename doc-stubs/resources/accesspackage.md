---
title: "accessPackage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackage resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackages](../api/accesspackage-list.md)|[accessPackage](../resources/accesspackage.md) collection|Get a list of the [accessPackage](../resources/accesspackage.md) objects and their properties.|
|[Create accessPackage](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Create a new [accessPackage](../resources/accesspackage.md) object.|
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.|
|[Update accessPackage](../api/accesspackage-update.md)|[accessPackage](../resources/accesspackage.md)|Update the properties of an [accessPackage](../resources/accesspackage.md) object.|
|[Delete accessPackage](../api/accesspackage-delete.md)|None|Deletes an [accessPackage](../resources/accesspackage.md) object.|
|[List accessPackageCatalog](../api/accesspackage-list-catalog.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|Get the accessPackageCatalog resources from the catalog navigation property.|
|[Add accessPackageCatalog](../api/accesspackage-post-catalog.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Add catalog by posting to the catalog collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isHidden|Boolean|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isHidden": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```

