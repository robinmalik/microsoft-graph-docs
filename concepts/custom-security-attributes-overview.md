---
title: "Overview of the custom security attributes API (Preview)"
description: "Learn about the custom security attributes API to programmatically define and assign your own business-specific attributes to Azure AD objects."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: conceptualPageType
---

# Overview of the custom security attributes API (Preview)

> [!IMPORTANT]
> The custom security attributes feature is currently in Preview. See the [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) for legal terms that apply to Azure features that are in beta, preview, or otherwise not yet released into general availability.

Custom security attributes in Azure Active Directory (Azure AD) are business-specific attributes that can be assigned to Azure AD directory objects. These attributes can be used to store sensitive information, categorize objects, or enforce fine-grained access control over specific Azure AD resources. Custom security attributes are a feature of [Azure AD attribute-based access control (ABAC)]().

Custom security attributes are configured using the [custom security attributes API](/graph/api/resources/customsecurityattributedefinition) in Microsoft Graph.

The following are the building blocks of the custom security attributes API:
+ Attribute sets—Represented by the [attributeSet](attributeset.md) resource type.
+ Custom security attribute definitions—Represented by the [customSecurityAttributeDefinition](customsecurityattributedefinition.md) resource type.
+ Allowed values—Represented by the [allowedValue](allowedvalue.md) resource type.

## Key resource types in the custom security attributes API

### Attribute sets

Attribute sets are a collection of custom security attributes whose management can be delegated to other users. The following are the general characteristics of **attributeSet** objects:

+ Up to 100 attributeSet objects can be defined in the tenant.
+ Attribute set identifiers can be up to 32 characters long, include Unicode characters, and can't contain spaces or special characters. The identifiers cannot be updated.

To configure attribute sets, use the [attributeSet](attributeset.md) resource type.
 
### Custom security attribute definitions

Custom security attribute definitions are a collection of key-value pairs that make up the schema of attribute sets. For example, the custom security attribute name, description, data type, and values. The following are the general characteristics of **customSecurityAttributeDefinition** objects:

+ Up to 500 active customSecurityAttributeDefinition objects can be defined in an attributeSet.
+ The objects can't be deleted, but can be deactivated. There's no limit to the number of deactivated objects in a tenant.

To configure custom security attribute definitions, use the [customSecurityAttributeDefinition](customsecurityattributedefinition.md) resource type.

### Allowed values

Allowed values represent the values that are assignable to a **customSecurityAttributeDefinition**. The following are the general characteristics of **allowedValue** objects:

+ Each customSecurityAttributeDefinition object can be assigned up to 50 active allowedValue objects.
+ Allowed values can't be deleted, but can be deactivated. There's no limit to the number of deactivated objects in a customSecurityAttributeDefinition.
+ Allowed values can be of Boolean, Integer, or String data types.
+ Allowed values can either be user-defined free-form values or predefined values.
+ Up to 100 predefined allowedValue objects can be added to a customSecurityAttributeDefinition object.

To configure attribute sets, use the [allowedValue](allowedvalue.md) resource type.

## Which directory objects support custom security attributes?

Custom security attributes can be assigned to only [user](user.md) and [servicePrincipal](serviceprincipal.md) objects through the **customSecurityAttributes** property. Users synced from an on-premises Active Directory can also be assigned custom security attributes.

## License requirements

Using the custom security attributes API requires an Azure AD Premium P1 or P2 license.

## Permissions

To call the custom security attributes API, you must have the appropriate [custom security attributes permissions](/graph/permissions-reference#custom-security-attributes-permissions).

The signed-in user must be in one of the following [Azure AD roles](/azure/active-directory/roles/permissions-reference) to manage custom security attributes.

+ [Attribute Definition Reader](/azure/active-directory/roles/permissions-reference#attribute-definition-reader)
+ [Attribute Definition Administrator](/azure/active-directory/roles/permissions-reference#attribute-definition-administrator)
+ [Attribute Assignment Reader](/azure/active-directory/roles/permissions-reference#attribute-assignment-reader)
+ [Attribute Assignment Administrator](/azure/active-directory/roles/permissions-reference#attribute-assignment-administrator)

By default, Global Administrator and other administrator roles don't have permissions to read, define, or assign custom security attributes.

## Next steps

+ [Custom security attributes API](/graph/api/resources/customsecurityattributedefinition)
+ [What are custom security attributes in Azure AD?](/azure/active-directory/fundamentals/custom-security-attributes-overview)
+ [Assign, remove, and filter custom security attributes using the Microsoft Graph API](/graph/howto-customsecurityattributes)
+ [Azure AD attribute-based access control (ABAC)]()