---
title: "accessPackageAssignmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageAssignmentRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get a list of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects and their properties.|
|[Create accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Get accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Read the properties and relationships of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Update accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-update.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Update the properties of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[Delete accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|None|Deletes an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.|
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|**TODO: Add Description**|
|[cancel](../api/accesspackageassignmentrequest-cancel.md)|None|**TODO: Add Description**|
|[List accessPackage](../api/accesspackageassignmentrequest-list-accesspackage.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackage resources from the accessPackage navigation property.|
|[Add accessPackage](../api/accesspackageassignmentrequest-post-accesspackage.md)|[accessPackage](../resources/accesspackage.md)|Add accessPackage by posting to the accessPackage collection.|
|[List accessPackageAssignment](../api/accesspackageassignmentrequest-list-assignment.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get the accessPackageAssignment resources from the assignment navigation property.|
|[Add accessPackageAssignment](../api/accesspackageassignmentrequest-post-assignment.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Add assignment by posting to the assignment collection.|
|[List accessPackageSubject](../api/accesspackageassignmentrequest-list-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get the accessPackageSubject resources from the requestor navigation property.|
|[Add accessPackageSubject](../api/accesspackageassignmentrequest-post-requestor.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Add requestor by posting to the requestor collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|requestType|accessPackageRequestType|**TODO: Add Description**. The possible values are: `notSpecified`, `userAdd`, `userUpdate`, `userRemove`, `adminAdd`, `adminUpdate`, `adminRemove`, `systemAdd`, `systemUpdate`, `systemRemove`, `onBehalfAdd`, `unknownFutureValue`.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|**TODO: Add Description**|
|state|accessPackageRequestState|**TODO: Add Description**. The possible values are: `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`.|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|**TODO: Add Description**|
|assignment|[accessPackageAssignment](../resources/accesspackageassignment.md)|**TODO: Add Description**|
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "state": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```

