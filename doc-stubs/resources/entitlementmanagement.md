---
title: "entitlementManagement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# entitlementManagement resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List entitlementManagements](../api/entitlementmanagement-list.md)|[entitlementManagement](../resources/entitlementmanagement.md) collection|Get a list of the [entitlementManagement](../resources/entitlementmanagement.md) objects and their properties.|
|[Create entitlementManagement](../api/identitygovernance-post-entitlementmanagement.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Create a new [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[Get entitlementManagement](../api/entitlementmanagement-get.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Read the properties and relationships of an [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[Update entitlementManagement](../api/entitlementmanagement-update.md)|[entitlementManagement](../resources/entitlementmanagement.md)|Update the properties of an [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[Delete entitlementManagement](../api/entitlementmanagement-delete.md)|None|Deletes an [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[List accessPackages](../api/entitlementmanagement-list-accesspackages.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackage resources from the accessPackages navigation property.|
|[Create accessPackage](../api/entitlementmanagement-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Create a new accessPackage object.|
|[List assignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get the accessPackageAssignmentRequest resources from the assignmentRequests navigation property.|
|[Create accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Create a new accessPackageAssignmentRequest object.|
|[List assignments](../api/entitlementmanagement-list-assignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get the accessPackageAssignment resources from the assignments navigation property.|
|[Create accessPackageAssignment](../api/entitlementmanagement-post-assignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Create a new accessPackageAssignment object.|
|[List catalogs](../api/entitlementmanagement-list-catalogs.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|Get the accessPackageCatalog resources from the catalogs navigation property.|
|[Create accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Create a new accessPackageCatalog object.|
|[List connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md)|[connectedOrganization](../resources/connectedorganization.md) collection|Get the connectedOrganization resources from the connectedOrganizations navigation property.|
|[Create connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)|[connectedOrganization](../resources/connectedorganization.md)|Create a new connectedOrganization object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackages|[accessPackage](../resources/accesspackage.md) collection|**TODO: Add Description**|
|assignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|**TODO: Add Description**|
|assignments|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|**TODO: Add Description**|
|catalogs|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|**TODO: Add Description**|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) collection|**TODO: Add Description**|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "String (identifier)"
}
```

