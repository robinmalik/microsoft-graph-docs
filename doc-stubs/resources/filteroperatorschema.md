---
title: "filterOperatorSchema resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# filterOperatorSchema resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List filterOperatorSchemas](../api/filteroperatorschema-list.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection|Get a list of the [filterOperatorSchema](../resources/filteroperatorschema.md) objects and their properties.|
|[Create filterOperatorSchema](../api/filteroperatorschema-post-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Create a new [filterOperatorSchema](../resources/filteroperatorschema.md) object.|
|[Get filterOperatorSchema](../api/filteroperatorschema-get.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Read the properties and relationships of a [filterOperatorSchema](../resources/filteroperatorschema.md) object.|
|[Update filterOperatorSchema](../api/filteroperatorschema-update.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Update the properties of a [filterOperatorSchema](../resources/filteroperatorschema.md) object.|
|[Delete filterOperatorSchema](../api/filteroperatorschema-delete.md)|None|Deletes a [filterOperatorSchema](../resources/filteroperatorschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|arity|scopeOperatorType|**TODO: Add Description**. The possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|scopeOperatorMultiValuedComparisonType|**TODO: Add Description**. The possible values are: `All`, `Any`.|
|name|String|**TODO: Add Description**|
|supportedAttributeTypes|attributeType collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "name": "String",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```

