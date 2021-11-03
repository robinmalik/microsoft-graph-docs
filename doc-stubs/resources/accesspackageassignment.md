---
title: "accessPackageAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageAssignments](../api/accesspackageassignment-list.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get a list of the [accessPackageAssignment](../resources/accesspackageassignment.md) objects and their properties.|
|[Create accessPackageAssignment](../api/entitlementmanagement-post-assignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Create a new [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Read the properties and relationships of an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Update accessPackageAssignment](../api/accesspackageassignment-update.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Update the properties of an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Delete accessPackageAssignment](../api/accesspackageassignment-delete.md)|None|Deletes an [accessPackageAssignment](../resources/accesspackageassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|**TODO: Add Description**|
|state|accessPackageAssignmentState|**TODO: Add Description**. The possible values are: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`.|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|**TODO: Add Description**|
|target|[accessPackageSubject](../resources/accesspackagesubject.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "state": "String",
  "status": "String",
  "expiredDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```

