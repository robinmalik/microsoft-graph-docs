---
title: "Configure custom security attributes using the Microsoft Graph API"
description: "Learn how to use the custom security attributes API in Microsoft Graph to configure custom security attributes for directory objects."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: conceptualPageType
---

# Configure custom security attributes using the Microsoft Graph API

The [custom security attributes API](../resources/custom-security-attributes-overview.md) in Microsoft Graph allows an organization to define and assign business-specific attributes to users and service principal objects. These attributes are assigned through the customSecurityAttribute property and can be used to store sensitive information, categorize objects, or enforce fine-grained access control over specific Azure AD resources.

The following article provides example requests for assigning different types of custom security attributes to users and service principals . Custom security attributes can be assigned or updated only through a **PATCH** operation in an [Update user]() or [Update servicePrincipal]() request.

## Assign custom security attributes to users or service principals

### Example 1: Assign a custom security attribute with a String value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `ProjectDate`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of String type.

#### Request


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

### Example 2: Assign a custom security attribute with a collection of String values to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Project`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts a collection of values of String types.

#### Request

<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multistring"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project@odata.type":"#Collection(String)",
            "Project":["Baker","Cascade"]
        }
    }
}
```

### Example 6: Assign a custom security attribute with an integer value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `NumVendors`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of Integer type.

#### Request


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":4
        }
    }
}
```

### Example 7: Assign a custom security attribute with a collection of Integer values to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `CostCenter`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts a collection of values of Integer types.

#### Request


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_multiinteger"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "CostCenter@odata.type":"#Collection(Int32)",
            "CostCenter":[1001,1003]
        }
    }
}
```

### Example 8: Assign a custom security attribute with a Boolean value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Certification`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only a Boolean type. Attributes that accept Boolean types can't be collections.

#### Request


<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":true
        }
    }
}
```


### Example 9: Update a custom security attribute with an integer value for a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `NumVendors`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of Integer type.

#### Request


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_integer"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":8
        }
    }
}
```

### Example 10: Update a custom security attribute with a Boolean value for a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Certification`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only a Boolean type. Attributes that accept Boolean types can't be collections.

#### Request


<!-- {
  "blockType": "request",
  "name": "update_user_customsecurityattribute_boolean"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Certification":false
        }
    }
}
```

## Remove custom security attributes from users

The following examples illustrate how to remove custom security attributes from users and service principals. To remove a custom security attribute from an object, assign the customSecurityAttributeDefinition the value `null` (for single-valued types) or an empty collection (for collection types).

### Example 11: Remove a single-valued custom security attribute assignment from a user

In the following example, the custom security attribute to remove has the following settings:

+ The customSecurityAttributeDefinition object is named `ProjectDate`.
+ It belongs to an attributeSet group named `Engineering`.

#### Request


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_singlevalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":null
        }
    }
}
```


### Example 12: Remove a multi-valued custom security attribute assignment from a user

In the following example, the custom security attribute to remove has the following settings:

+ The customSecurityAttributeDefinition object is named `Project`.
+ It belongs to an attributeSet group named `Engineering`.

#### Request


<!-- {
  "blockType": "request",
  "name": "remove_user_customsecurityattribute_multivalue"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "Project":[]
        }
    }
}
```


## Next steps

+ [Custom security attributes API]()