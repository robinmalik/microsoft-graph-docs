---
title: "managementTemplateCollection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managementTemplateCollection resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/managedtenants-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateCollections](../api/managedtenants-managementtemplatecollection-list.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get a list of the [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) objects and their properties.|
|[Create managementTemplateCollection](../api/managedtenants-managementtemplate-post-managementtemplatecollections.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Create a new [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[Get managementTemplateCollection](../api/managedtenants-managementtemplatecollection-get.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Read the properties and relationships of a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[Update managementTemplateCollection](../api/managedtenants-managementtemplatecollection-update.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Update the properties of a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[Delete managementTemplateCollection](../api/managedtenants-managementtemplatecollection-delete.md)|None|Deletes a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[List managementTemplates](../api/managedtenants-managementtemplatecollection-list-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the managementTemplate resources from the managementTemplates navigation property.|
|[Add managementTemplate](../api/managedtenants-managementtemplatecollection-post-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Add managementTemplates by posting to the managementTemplates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/managedtenants-entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateCollection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplateCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```

