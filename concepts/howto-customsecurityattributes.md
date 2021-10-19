---
title: "Assign, remove, and filter custom security attributes using the Microsoft Graph API"
description: "Learn how to use the custom security attributes API in Microsoft Graph to configure custom security attributes for directory objects."
author: "rolyon"
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: "directory-management"
---

# Assign, remove, and filter custom security attributes using the Microsoft Graph API

The [custom security attributes API](../resources/custom-security-attributes-overview.md) in Microsoft Graph allows an organization to define and assign business-specific attributes to users and service principal objects. These attributes are assigned through the **customSecurityAttributes** property and can be used to store sensitive information, categorize objects, or enforce fine-grained access control over specific Azure AD resources.

This article provides examples for assigning different types of custom security attributes to users and service principals. Custom security attributes can be assigned or updated only through a **PATCH** operation in an [Update user]() or [Update servicePrincipal]() request.

>**NOTE**: The calling user must also be in the appropriate [Azure AD roles](../resources/howto-customsecurityattributes.md) to define, assign, unassign, or retrieve custom security attributes.

## Assign custom security attributes to users or service principals

### Example 1: Assign a custom security attribute with a String value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `ProjectDate`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of String data type.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```

### Example 2: Assign a custom security attribute with a collection of String values to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Project`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts a collection of values of String data types.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "Project@odata.type":"#Collection(String)",
            "Project":["Baker","Cascade"]
        }
    }
}
```

### Example 3: Assign a custom security attribute with an integer value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `NumVendors`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of Integer data type.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":4
        }
    }
}
```

### Example 4: Assign a custom security attribute with a collection of Integer values to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `CostCenter`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts a collection of values of Integer data types.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "CostCenter@odata.type":"#Collection(Int32)",
            "CostCenter":[1001,1003]
        }
    }
}
```

### Example 5: Assign a custom security attribute with a Boolean value to a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Certification`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only a Boolean data type. Attributes that accept Boolean types can't be collections.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "Certification":true
        }
    }
}
```


### Example 6: Update a custom security attribute with an integer value for a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `NumVendors`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only one value of Integer data type.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "NumVendors@odata.type":"#Int32",
            "NumVendors":8
        }
    }
}
```

### Example 7: Update a custom security attribute with a Boolean value for a user

In the following example, the custom security attribute has the following settings:

+ The customSecurityAttributeDefinition object is named `Certification`.
+ It belongs to an attributeSet group named `Engineering`.
+ It accepts only a Boolean data type. Attributes that accept Boolean types can't be collections.

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "Certification":false
        }
    }
}
```

## Remove custom security attributes from users

The following examples illustrate how to remove custom security attributes from users and service principals. To remove a custom security attribute from an object, assign the customSecurityAttributeDefinition object the value `null` (for single-valued types) or an empty collection (for collection types). This action automatically assigns the customSecurityAttributes property the value `null`.

### Example 8: Remove a single-valued custom security attribute assignment from a user

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "ProjectDate":null
        }
    }
}
```


### Example 9: Remove a multi-valued custom security attribute assignment from a user

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
            "@odata.type":"#microsoft.graph.CustomSecurityAttributeValue",
            "Project":[]
        }
    }
}
```

## Filter custom security attributes in user and servicePrincipal objects

The **customSecurityAttributes** property of the user and servicePrincipal directory objects supports `$filter` with the following operators: `eq`, `startsWith`, `NOT`, and `ne`. The following examples illustrate the syntax for filter queries.

### Example 10: $filter (eq) on a user object


### Example 11: $filter (ne) on a service principal object


### Example 12: $filter (NOT) on a service principal object


### Example 13: $filter (startsWith) on a user object



## Next steps

+ [Custom security attributes API](/graph/api/resources/customsecurityattributedefinition)