---
title: "emailAuthenticationMethod resource type"
description: "A representation of an email address registered to a user. Email is an authentication method available only to self-service password reset (SSPR)"
author: "tilarso"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# emailAuthenticationMethod resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A representation of an email address registered to a user. Email is an authentication method available only to self-service password reset (SSPR). Users may only have one email authentication method.

This is a derived type that inherits from the [authenticationMethod](authenticationmethod.md) resource type.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List emailMethods](../api/authentication-list-emailmethods.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection|Retrieve a list of a user's emailAuthenticationMethods. Users may only have one email authentication method.|
|[Create emailMethod](../api/authentication-post-emailmethods.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Create a user's emailMethod object.|
|[Get emailAuthenticationMethod](../api/emailauthenticationmethod-get.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Retrieve the properties  of the user's emailAuthenticationMethod object.|
|[Update emailAuthenticationMethod](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Update the properties of a user's emailMethods object.|
|[Delete emailAuthenticationMethod](../api/emailauthenticationmethod-delete.md)|None|Delete a user's emailAuthenticationMethod object.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The identifier of the email address registered to this user.|
|emailAddress|String|The email address registered to this user.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

