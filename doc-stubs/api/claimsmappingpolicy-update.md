---
title: "Update claimsMappingPolicy"
description: "Update the properties of a claimsMappingPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update claimsMappingPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.

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
PATCH /policyRoot/claimsMappingPolicies/{claimsMappingPolicyId}
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
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md). Required.|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md). Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policyRoot/claimsMappingPolicies/{claimsMappingPolicyId}
Content-Type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.claimsMappingPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
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
  "@odata.type": "#microsoft.graph.claimsMappingPolicy",
  "id": "984d6855-6855-984d-5568-4d9855684d98",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

