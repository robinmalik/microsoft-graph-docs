---
title: "Update tenantAppManagementPolicy"
description: "Update the properties of a tenantAppManagementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update tenantAppManagementPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) object.

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
PATCH /tenantAppManagementPolicy
PATCH /policyRoot/defaultAppManagementPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|isEnabled|Boolean|**TODO: Add Description** Required.|
|applicationRestrictions|[Microsoft.DirectoryServices.appManagementConfiguration](../resources/appmanagementconfiguration.md)|**TODO: Add Description** Optional.|
|servicePrincipalRestrictions|[Microsoft.DirectoryServices.appManagementConfiguration](../resources/appmanagementconfiguration.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tenantappmanagementpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantAppManagementPolicy
Content-Type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.tenantAppManagementPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "applicationRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.tenantAppManagementPolicy",
  "id": "1c3cc936-c936-1c3c-36c9-3c1c36c93c1c",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "applicationRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```

