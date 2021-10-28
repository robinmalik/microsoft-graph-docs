---
title: "Create application"
description: "Create a new application object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create application
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [application](../resources/application.md) object.

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
POST /applications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [application](../resources/application.md) object.

You can specify the following properties when creating an **application**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|api|[Microsoft.DirectoryServices.apiApplication](../resources/apiapplication.md)|**TODO: Add Description** Optional.|
|appId|String|**TODO: Add Description** Optional.|
|appMetadata|[Microsoft.DirectoryServices.appMetadata](../resources/appmetadata.md)|**TODO: Add Description** Optional.|
|appRoles|[Microsoft.DirectoryServices.appRole](../resources/approle.md) collection|**TODO: Add Description** Required.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|disabledByMicrosoftStatus|String|**TODO: Add Description** Optional.|
|isFallbackPublicClient|Boolean|**TODO: Add Description** Optional.|
|identifierUris|String collection|**TODO: Add Description** Required.|
|defaultRedirectUri|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|expectsForwardableIdTokens|Boolean|**TODO: Add Description** Optional.|
|groupMembershipClaims|String|**TODO: Add Description** Optional.|
|info|[Microsoft.DirectoryServices.informationalUrl](../resources/informationalurl.md)|**TODO: Add Description** Optional.|
|isDeviceOnlyAuthSupported|Boolean|**TODO: Add Description** Optional.|
|isManagementRestricted|Boolean|**TODO: Add Description** Optional.|
|keyCredentials|[Microsoft.DirectoryServices.keyCredential](../resources/keycredential.md) collection|**TODO: Add Description** Required.|
|legacyAllowPassthroughUsers|Boolean|**TODO: Add Description** Optional.|
|logo|Stream|**TODO: Add Description** Required.|
|microsoftPolicyGroup|Boolean|**TODO: Add Description** Optional.|
|notes|String|**TODO: Add Description** Optional.|
|optionalClaims|[Microsoft.DirectoryServices.optionalClaims](../resources/optionalclaims.md)|**TODO: Add Description** Optional.|
|parentalControlSettings|[Microsoft.DirectoryServices.parentalControlSettings](../resources/parentalcontrolsettings.md)|**TODO: Add Description** Optional.|
|passwordCredentials|[Microsoft.DirectoryServices.passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description** Required.|
|publicClient|[Microsoft.DirectoryServices.publicClientApplication](../resources/publicclientapplication.md)|**TODO: Add Description** Optional.|
|publisherDomain|String|**TODO: Add Description** Optional.|
|requiredResourceAccess|[Microsoft.DirectoryServices.requiredResourceAccess](../resources/requiredresourceaccess.md) collection|**TODO: Add Description** Required.|
|servicePrincipalLifecyclePolicy|String|**TODO: Add Description** Optional.|
|serviceTreeId|String|**TODO: Add Description** Optional.|
|signInAudience|String|**TODO: Add Description** Optional.|
|spa|[Microsoft.DirectoryServices.spaApplication](../resources/spaapplication.md)|**TODO: Add Description** Optional.|
|tags|String collection|**TODO: Add Description** Required.|
|tokenEncryptionKeyId|Guid|**TODO: Add Description** Optional.|
|trustedSubjectNameAndIssuers|[Microsoft.DirectoryServices.trustedSubjectNameAndIssuer](../resources/trustedsubjectnameandissuer.md) collection|**TODO: Add Description** Optional.|
|uniqueName|String|**TODO: Add Description** Optional.|
|verifiedPublisher|[Microsoft.DirectoryServices.verifiedPublisher](../resources/verifiedpublisher.md)|**TODO: Add Description** Optional.|
|web|[Microsoft.DirectoryServices.webApplication](../resources/webapplication.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [application](../resources/application.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications
Content-Type: application/json
Content-length: 2124

{
  "@odata.type": "#Microsoft.DirectoryServices.application",
  "deletedDateTime": "String (timestamp)",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication"
  },
  "appId": "String",
  "appMetadata": {
    "@odata.type": "microsoft.graph.appMetadata"
  },
  "appRoles": [
    {
      "@odata.type": "microsoft.graph.appRole"
    }
  ],
  "description": "String",
  "disabledByMicrosoftStatus": "String",
  "isFallbackPublicClient": "Boolean",
  "identifierUris": [
    "String"
  ],
  "defaultRedirectUri": "String",
  "displayName": "String",
  "expectsForwardableIdTokens": "Boolean",
  "groupMembershipClaims": "String",
  "info": {
    "@odata.type": "microsoft.graph.informationalUrl"
  },
  "isDeviceOnlyAuthSupported": "Boolean",
  "isManagementRestricted": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "legacyAllowPassthroughUsers": "Boolean",
  "logo": "Stream",
  "microsoftPolicyGroup": "Boolean",
  "notes": "String",
  "optionalClaims": {
    "@odata.type": "microsoft.graph.optionalClaims"
  },
  "parentalControlSettings": {
    "@odata.type": "microsoft.graph.parentalControlSettings"
  },
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredential"
    }
  ],
  "publicClient": {
    "@odata.type": "microsoft.graph.publicClientApplication"
  },
  "publisherDomain": "String",
  "requiredResourceAccess": [
    {
      "@odata.type": "microsoft.graph.requiredResourceAccess"
    }
  ],
  "servicePrincipalLifecyclePolicy": "String",
  "serviceTreeId": "String",
  "signInAudience": "String",
  "spa": {
    "@odata.type": "microsoft.graph.spaApplication"
  },
  "tags": [
    "String"
  ],
  "tokenEncryptionKeyId": "Guid",
  "trustedSubjectNameAndIssuers": [
    {
      "@odata.type": "microsoft.graph.trustedSubjectNameAndIssuer"
    }
  ],
  "uniqueName": "String",
  "verifiedPublisher": {
    "@odata.type": "microsoft.graph.verifiedPublisher"
  },
  "web": {
    "@odata.type": "microsoft.graph.webApplication"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.application"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.application",
  "id": "ea8c5f2a-5f2a-ea8c-2a5f-8cea2a5f8cea",
  "deletedDateTime": "String (timestamp)",
  "api": {
    "@odata.type": "microsoft.graph.apiApplication"
  },
  "appId": "String",
  "appMetadata": {
    "@odata.type": "microsoft.graph.appMetadata"
  },
  "appRoles": [
    {
      "@odata.type": "microsoft.graph.appRole"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "disabledByMicrosoftStatus": "String",
  "isFallbackPublicClient": "Boolean",
  "identifierUris": [
    "String"
  ],
  "defaultRedirectUri": "String",
  "displayName": "String",
  "expectsForwardableIdTokens": "Boolean",
  "groupMembershipClaims": "String",
  "info": {
    "@odata.type": "microsoft.graph.informationalUrl"
  },
  "isDeviceOnlyAuthSupported": "Boolean",
  "isManagementRestricted": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "legacyAllowPassthroughUsers": "Boolean",
  "logo": "Stream",
  "microsoftPolicyGroup": "Boolean",
  "notes": "String",
  "optionalClaims": {
    "@odata.type": "microsoft.graph.optionalClaims"
  },
  "parentalControlSettings": {
    "@odata.type": "microsoft.graph.parentalControlSettings"
  },
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredential"
    }
  ],
  "publicClient": {
    "@odata.type": "microsoft.graph.publicClientApplication"
  },
  "publisherDomain": "String",
  "requiredResourceAccess": [
    {
      "@odata.type": "microsoft.graph.requiredResourceAccess"
    }
  ],
  "servicePrincipalLifecyclePolicy": "String",
  "serviceTreeId": "String",
  "signInAudience": "String",
  "spa": {
    "@odata.type": "microsoft.graph.spaApplication"
  },
  "tags": [
    "String"
  ],
  "tokenEncryptionKeyId": "Guid",
  "trustedSubjectNameAndIssuers": [
    {
      "@odata.type": "microsoft.graph.trustedSubjectNameAndIssuer"
    }
  ],
  "uniqueName": "String",
  "verifiedPublisher": {
    "@odata.type": "microsoft.graph.verifiedPublisher"
  },
  "web": {
    "@odata.type": "microsoft.graph.webApplication"
  }
}
```

