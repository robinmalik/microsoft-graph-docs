---
title: "Create directoryDefinition"
description: "Create a new directoryDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create directoryDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [directoryDefinition](../resources/directorydefinition.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [directoryDefinition](../resources/directorydefinition.md) object.

You can specify the following properties when creating a **directoryDefinition**.

|Property|Type|Description|
|:---|:---|:---|
|discoveryDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|discoverabilities|directoryDefinitionDiscoverabilities|**TODO: Add Description**. The possible values are: `None`, `AttributeNames`, `AttributeDataTypes`, `AttributeReadOnly`, `ReferenceAttributes`, `UnknownFutureValue`. Required.|
|name|String|**TODO: Add Description** Optional.|
|objects|[microsoft.synchronization.objectDefinition](../resources/objectdefinition.md) collection|**TODO: Add Description** Optional.|
|readOnly|Boolean|**TODO: Add Description** Required.|
|version|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [directoryDefinition](../resources/directorydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_directorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/schema/directories
Content-Type: application/json
Content-length: 315

{
  "@odata.type": "#microsoft.synchronization.directoryDefinition",
  "discoveryDateTime": "String (timestamp)",
  "discoverabilities": "String",
  "name": "String",
  "objects": [
    {
      "@odata.type": "microsoft.graph.objectDefinition"
    }
  ],
  "readOnly": "Boolean",
  "version": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.synchronization.directoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.synchronization.directoryDefinition",
  "id": "48e513d6-13d6-48e5-d613-e548d613e548",
  "discoveryDateTime": "String (timestamp)",
  "discoverabilities": "String",
  "name": "String",
  "objects": [
    {
      "@odata.type": "microsoft.graph.objectDefinition"
    }
  ],
  "readOnly": "Boolean",
  "version": "String"
}
```

