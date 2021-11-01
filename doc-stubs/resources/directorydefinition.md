---
title: "directoryDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directoryDefinition resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List directoryDefinitions](../api/directorydefinition-list.md)|[directoryDefinition](../resources/directorydefinition.md) collection|Get a list of the [directoryDefinition](../resources/directorydefinition.md) objects and their properties.|
|[Create directoryDefinition](../api/synchronizationschema-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Create a new [directoryDefinition](../resources/directorydefinition.md) object.|
|[Get directoryDefinition](../api/directorydefinition-get.md)|[directoryDefinition](../resources/directorydefinition.md)|Read the properties and relationships of a [directoryDefinition](../resources/directorydefinition.md) object.|
|[Update directoryDefinition](../api/directorydefinition-update.md)|[directoryDefinition](../resources/directorydefinition.md)|Update the properties of a [directoryDefinition](../resources/directorydefinition.md) object.|
|[Delete directoryDefinition](../api/directorydefinition-delete.md)|None|Deletes a [directoryDefinition](../resources/directorydefinition.md) object.|
|[discover](../api/directorydefinition-discover.md)|[directoryDefinition](../resources/directorydefinition.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|discoverabilities|directoryDefinitionDiscoverabilities|**TODO: Add Description**. The possible values are: `None`, `AttributeNames`, `AttributeDataTypes`, `AttributeReadOnly`, `ReferenceAttributes`, `UnknownFutureValue`.|
|discoveryDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|objects|[objectDefinition](../resources/objectdefinition.md) collection|**TODO: Add Description**|
|readOnly|Boolean|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "id": "String (identifier)",
  "discoveryDateTime": "String (timestamp)",
  "discoverabilities": "String",
  "name": "String",
  "objects": [
    {
      "@odata.type": "microsoft.graph.objectDefinition"
    }
  ],
  "readOnly": "Boolean",
  "version": "String"
}
```

