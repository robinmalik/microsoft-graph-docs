---
title: "managementTemplateCollection resource type"
description: "Represents a collection of management templates."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementTemplateCollection resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a collection of management templates.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managementTemplateCollections](../api/managedtenants-managementtemplatecollection-list.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) collection|Get a list of the [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) objects and their properties.|
|[Get managementTemplateCollection](../api/managedtenants-managementtemplatecollection-get.md)|[microsoft.graph.managedTenants.managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md)|Read the properties and relationships of a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.|
|[List managementTemplates](../api/managedtenants-managementtemplatecollection-list-managementtemplates.md)|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|Get the managementTemplate resources from the managementTemplates navigation property.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description for the management template collection. Required. Optional.|
|displayName|String|The display name for the management template collection. Required. Optional.|
|id|String|The unique identifier for the management template collection. Required. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection|The management template associated with this management template collection. Required. Read-only.|

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
