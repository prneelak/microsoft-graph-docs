---
title: "Add multiValueExtendedProperties"
description: "Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add multiValueExtendedProperties

Namespace: microsoft.graph

Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.

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
POST /me/contactFolders/{contactFolderId}/multiValueExtendedProperties/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_multivaluelegacyextendedproperty_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/contactFolders/{contactFolderId}/multiValueExtendedProperties
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "value": [
    "Value value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "id": "c1905024-5024-c190-2450-90c1245090c1",
  "value": [
    "Value value"
  ]
}
```

