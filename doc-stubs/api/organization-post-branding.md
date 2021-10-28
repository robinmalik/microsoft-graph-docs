---
title: "Create organizationalBranding"
description: "Create a new organizationalBranding object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create organizationalBranding
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [organizationalBranding](../resources/organizationalbranding.md) object.

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
POST ** Collection URI for Microsoft.DirectoryServices.organizationalBranding not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [organizationalBranding](../resources/organizationalbranding.md) object.

You can specify the following properties when creating an **organizationalBranding**.

|Property|Type|Description|
|:---|:---|:---|
|backgroundColor|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|backgroundImage|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|backgroundImageRelativeUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|bannerLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|bannerLogoRelativeUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|cdnList|String collection|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|signInPageText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|squareLogo|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|squareLogoRelativeUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|usernameHintText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customAccountResetCredentialsUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customCannotAccessYourAccountText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customCannotAccessYourAccountUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customForgotMyPasswordText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customPrivacyAndCookiesText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customPrivacyAndCookiesUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customResetItNowText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customTermsOfUseText|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|customTermsOfUseUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|favicon|Stream|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|faviconRelativeUrl|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|headerBackgroundColor|String|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|
|loginPageTextVisibilitySettings|[Microsoft.DirectoryServices.loginPageTextVisibilitySettings](../resources/loginpagetextvisibilitysettings.md)|**TODO: Add Description** Inherited from [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md). Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [organizationalBranding](../resources/organizationalbranding.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_organizationalbranding_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.organizationalBranding not found
Content-Type: application/json
Content-length: 1014

{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBranding",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String",
  "customAccountResetCredentialsUrl": "String",
  "customCannotAccessYourAccountText": "String",
  "customCannotAccessYourAccountUrl": "String",
  "customForgotMyPasswordText": "String",
  "customPrivacyAndCookiesText": "String",
  "customPrivacyAndCookiesUrl": "String",
  "customResetItNowText": "String",
  "customTermsOfUseText": "String",
  "customTermsOfUseUrl": "String",
  "favicon": "Stream",
  "faviconRelativeUrl": "String",
  "headerBackgroundColor": "String",
  "loginPageTextVisibilitySettings": {
    "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.organizationalBranding"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.organizationalBranding",
  "id": "e453da84-da84-e453-84da-53e484da53e4",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String",
  "customAccountResetCredentialsUrl": "String",
  "customCannotAccessYourAccountText": "String",
  "customCannotAccessYourAccountUrl": "String",
  "customForgotMyPasswordText": "String",
  "customPrivacyAndCookiesText": "String",
  "customPrivacyAndCookiesUrl": "String",
  "customResetItNowText": "String",
  "customTermsOfUseText": "String",
  "customTermsOfUseUrl": "String",
  "favicon": "Stream",
  "faviconRelativeUrl": "String",
  "headerBackgroundColor": "String",
  "loginPageTextVisibilitySettings": {
    "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
  }
}
```

