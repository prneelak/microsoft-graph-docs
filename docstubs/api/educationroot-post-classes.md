---
title: "Add classes"
description: "Add classes by posting to the classes collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add classes

Namespace: microsoft.graph

Add classes by posting to the classes collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /education/classes/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationClass](../resources/educationclass.md) object.

The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|mailNickname|String||
|description|String||
|createdBy|[identitySet](../resources/identityset.md)||
|classCode|String||
|externalName|String||
|externalId|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](../resources/educationterm.md)||



## Response
If successful, this method returns a `201 Created` response code and a [educationClass](../resources/educationclass.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/education/classes
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "Display Name value",
  "mailNickname": "Mail Nickname value",
  "description": "Description value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "classCode": "Class Code value",
  "externalName": "External Name value",
  "externalId": "External Id value",
  "externalSource": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationclass"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 818

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "9457bab8-bab8-9457-b8ba-5794b8ba5794",
  "displayName": "Display Name value",
  "mailNickname": "Mail Nickname value",
  "description": "Description value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "classCode": "Class Code value",
  "externalName": "External Name value",
  "externalId": "External Id value",
  "externalSource": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  }
}
```

