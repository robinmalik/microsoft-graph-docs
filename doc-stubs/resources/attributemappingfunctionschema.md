---
title: "attributeMappingFunctionSchema resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attributeMappingFunctionSchema resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List attributeMappingFunctionSchemas](../api/attributemappingfunctionschema-list.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection|Get a list of the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) objects and their properties.|
|[Create attributeMappingFunctionSchema](../api/attributemappingfunctionschema-post-functions.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md)|Create a new [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|
|[Get attributeMappingFunctionSchema](../api/attributemappingfunctionschema-get.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md)|Read the properties and relationships of an [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|
|[Update attributeMappingFunctionSchema](../api/attributemappingfunctionschema-update.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md)|Update the properties of an [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|
|[Delete attributeMappingFunctionSchema](../api/attributemappingfunctionschema-delete.md)|None|Deletes an [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String|**TODO: Add Description**|
|parameters|[attributeMappingParameterSchema](../resources/attributemappingparameterschema.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
  "name": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
    }
  ]
}
```

