---
title: "accessPackageSubject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageSubject resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageSubjects](../api/accesspackagesubject-list.md)|[accessPackageSubject](../resources/accesspackagesubject.md) collection|Get a list of the [accessPackageSubject](../resources/accesspackagesubject.md) objects and their properties.|
|[Create accessPackageSubject](../api/accesspackageassignment-post-target.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Create a new [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read the properties and relationships of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Update accessPackageSubject](../api/accesspackagesubject-update.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Update the properties of an [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[Delete accessPackageSubject](../api/accesspackagesubject-delete.md)|None|Deletes an [accessPackageSubject](../resources/accesspackagesubject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|objectId|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|subjectType|accessPackageSubjectType|**TODO: Add Description**. The possible values are: `notSpecified`, `user`, `servicePrincipal`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectedOrganization|[connectedOrganization](../resources/connectedorganization.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "objectId": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "onPremisesSecurityIdentifier": "String",
  "subjectType": "String"
}
```

