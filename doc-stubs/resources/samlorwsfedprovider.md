---
title: "samlOrWsFedProvider resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# samlOrWsFedProvider resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.


Inherits from [identityProviderBase](../resources/identityproviderbase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List samlOrWsFedProviders](../api/samlorwsfedprovider-list.md)|[samlOrWsFedProvider](../resources/samlorwsfedprovider.md) collection|Get a list of the [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) objects and their properties.|
|[Get samlOrWsFedProvider](../api/samlorwsfedprovider-get.md)|[samlOrWsFedProvider](../resources/samlorwsfedprovider.md)|Read the properties and relationships of a [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) object.|
|[Update samlOrWsFedProvider](../api/samlorwsfedprovider-update.md)|[samlOrWsFedProvider](../resources/samlorwsfedprovider.md)|Update the properties of a [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) object.|
|[Delete samlOrWsFedProvider](../api/samlorwsfedprovider-delete.md)|None|Deletes a [samlOrWsFedProvider](../resources/samlorwsfedprovider.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md).|
|id|String|**TODO: Add Description** Inherited from [identityProviderBase](../resources/identityproviderbase.md).|
|issuerUri|String|**TODO: Add Description**|
|metadataExchangeUri|String|**TODO: Add Description**|
|passiveSignInUri|String|**TODO: Add Description**|
|preferredAuthenticationProtocol|authenticationProtocol|**TODO: Add Description**. The possible values are: `wsFed`, `saml`, `unknownFutureValue`.|
|signingCertificate|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.samlOrWsFedProvider",
  "baseType": "Microsoft.DirectoryServices.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.samlOrWsFedProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "issuerUri": "String",
  "metadataExchangeUri": "String",
  "signingCertificate": "String",
  "passiveSignInUri": "String",
  "preferredAuthenticationProtocol": "String"
}
```

