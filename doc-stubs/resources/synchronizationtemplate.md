---
title: "synchronizationTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationTemplate resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizationTemplates](../api/synchronizationtemplate-list.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|Get a list of the [synchronizationTemplate](../resources/synchronizationtemplate.md) objects and their properties.|
|[Create synchronizationTemplate](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Create a new [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Read the properties and relationships of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Update synchronizationTemplate](../api/synchronizationtemplate-update.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Delete synchronizationTemplate](../api/synchronizationtemplate-delete.md)|None|Deletes a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[List synchronizationSchema](../api/synchronizationtemplate-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchema resources from the schema navigation property.|
|[Create synchronizationSchema](../api/synchronizationtemplate-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new synchronizationSchema object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationId|Guid|**TODO: Add Description**|
|default|Boolean|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoverable|Boolean|**TODO: Add Description**|
|factoryTag|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|metadata|[metadataEntry](../resources/metadataentry.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "id": "String (identifier)",
  "applicationId": "Guid",
  "default": "Boolean",
  "description": "String",
  "discoverable": "Boolean",
  "factoryTag": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry"
    }
  ]
}
```

