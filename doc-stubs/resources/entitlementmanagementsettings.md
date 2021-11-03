---
title: "entitlementManagementSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# entitlementManagementSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List entitlementManagementSettings](../api/entitlementmanagementsettings-list.md)|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md) collection|Get a list of the [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) objects and their properties.|
|[Create entitlementManagementSettings](../api/entitlementmanagement-post-settings.md)|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Create a new [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.|
|[Get entitlementManagementSettings](../api/entitlementmanagementsettings-get.md)|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Read the properties and relationships of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.|
|[Update entitlementManagementSettings](../api/entitlementmanagementsettings-update.md)|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Update the properties of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.|
|[Delete entitlementManagementSettings](../api/entitlementmanagementsettings-delete.md)|None|Deletes an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|durationUntilExternalUserDeletedAfterBlocked|Duration|**TODO: Add Description**|
|externalUserLifecycleAction|accessPackageExternalUserLifecycleAction|**TODO: Add Description**. The possible values are: `none`, `blockSignIn`, `blockSignInAndDelete`, `unknownFutureValue`.|
|id|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSettings",
  "id": "String (identifier)",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```

