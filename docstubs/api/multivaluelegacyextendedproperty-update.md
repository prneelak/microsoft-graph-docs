---
title: "Update multiValueLegacyExtendedProperty"
description: "Update the properties of a multiValueLegacyExtendedProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update multiValueLegacyExtendedProperty

Namespace: microsoft.graph

Update the properties of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

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
PATCH /me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/contacts/{contactId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/mailFolders/{mailFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/contactFolders/{contactFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
PATCH /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_multivaluelegacyextendedproperty"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

