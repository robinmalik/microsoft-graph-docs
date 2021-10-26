---
title: "graphAPIErrorDetails resource type"
description: "Represents the error details for a Microsoft Graph that can occur with specific managed tenant operations."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# graphAPIErrorDetails resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the error details for a Microsoft Graph that can occur with specific managed tenant operations.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|The error code for the given error.|
|message|String|The error message for the given error.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.graphAPIErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.graphAPIErrorDetails",
  "code": "String",
  "message": "String"
}
```
