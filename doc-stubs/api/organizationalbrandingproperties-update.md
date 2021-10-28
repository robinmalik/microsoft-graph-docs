---
title: "Update organizationalBrandingProperties"
description: "Update the properties of an organizationalBrandingProperties object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update organizationalBrandingProperties
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.

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
PATCH /organizationalBrandingProperties
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
|backgroundColor|String|**TODO: Add Description** Optional.|
|backgroundImage|Stream|**TODO: Add Description** Optional.|
|backgroundImageRelativeUrl|String|**TODO: Add Description** Optional.|
|bannerLogo|Stream|**TODO: Add Description** Optional.|
|bannerLogoRelativeUrl|String|**TODO: Add Description** Optional.|
|cdnList|String collection|**TODO: Add Description** Optional.|
|signInPageText|String|**TODO: Add Description** Optional.|
|squareLogo|Stream|**TODO: Add Description** Optional.|
|squareLogoRelativeUrl|String|**TODO: Add Description** Optional.|
|usernameHintText|String|**TODO: Add Description** Optional.|
|customAccountResetCredentialsUrl|String|**TODO: Add Description** Optional.|
|customCannotAccessYourAccountText|String|**TODO: Add Description** Optional.|
|customCannotAccessYourAccountUrl|String|**TODO: Add Description** Optional.|
|customForgotMyPasswordText|String|**TODO: Add Description** Optional.|
|customPrivacyAndCookiesText|String|**TODO: Add Description** Optional.|
|customPrivacyAndCookiesUrl|String|**TODO: Add Description** Optional.|
|customResetItNowText|String|**TODO: Add Description** Optional.|
|customTermsOfUseText|String|**TODO: Add Description** Optional.|
|customTermsOfUseUrl|String|**TODO: Add Description** Optional.|
|favicon|Stream|**TODO: Add Description** Optional.|
|faviconRelativeUrl|String|**TODO: Add Description** Optional.|
|headerBackgroundColor|String|**TODO: Add Description** Optional.|
|loginPageTextVisibilitySettings|[Microsoft.DirectoryServices.loginPageTextVisibilitySettings](../resources/loginpagetextvisibilitysettings.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organizationalBrandingProperties
Content-Type: application/json
Content-length: 1012

{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
  "id": "f8b5d263-d263-f8b5-63d2-b5f863d2b5f8",
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

