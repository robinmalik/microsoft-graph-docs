---
title: "roleManagement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleManagement resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleManagements](../api/rolemanagement-list.md)|[roleManagement](../resources/rolemanagement.md) collection|Get a list of the [roleManagement](../resources/rolemanagement.md) objects and their properties.|
|[Get roleManagement](../api/rolemanagement-get.md)|[roleManagement](../resources/rolemanagement.md)|Read the properties and relationships of a [roleManagement](../resources/rolemanagement.md) object.|
|[Update roleManagement](../api/rolemanagement-update.md)|[roleManagement](../resources/rolemanagement.md)|Update the properties of a [roleManagement](../resources/rolemanagement.md) object.|
|[Delete roleManagement](../api/rolemanagement-delete.md)|None|Deletes a [roleManagement](../resources/rolemanagement.md) object.|
|[List rbacApplication](../api/rolemanagement-list-entitlementmanagement.md)|[rbacApplication](../resources/rbacapplication.md) collection|Get the rbacApplication resources from the entitlementManagement navigation property.|
|[Create rbacApplication](../api/rolemanagement-post-entitlementmanagement.md)|[rbacApplication](../resources/rbacapplication.md)|Create a new rbacApplication object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|entitlementManagement|[rbacApplication](../resources/rbacapplication.md)|The RbacApplication for Entitlement Management|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

