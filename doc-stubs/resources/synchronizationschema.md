---
title: "synchronizationSchema resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationSchema resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizationSchemas](../api/synchronizationschema-list.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get a list of the [synchronizationSchema](../resources/synchronizationschema.md) objects and their properties.|
|[Create synchronizationSchema](../api/synchronizationjob-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Update synchronizationSchema](../api/synchronizationschema-update.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Delete synchronizationSchema](../api/synchronizationschema-delete.md)|None|Deletes a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[functions](../api/synchronizationschema-functions.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection|**TODO: Add Description**|
|[filterOperators](../api/synchronizationschema-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection|**TODO: Add Description**|
|[parseExpression](../api/synchronizationschema-parseexpression.md)|[parseExpressionResponse](../resources/parseexpressionresponse.md)|**TODO: Add Description**|
|[List directories](../api/synchronizationschema-list-directories.md)|[directoryDefinition](../resources/directorydefinition.md) collection|Get the directoryDefinition resources from the directories navigation property.|
|[Create directoryDefinition](../api/synchronizationschema-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Create a new directoryDefinition object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|synchronizationRules|[synchronizationRule](../resources/synchronizationrule.md) collection|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directories|[directoryDefinition](../resources/directorydefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```

