---
title: "Update singleValueLegacyExtendedProperty"
description: "Update the properties of a singleValueLegacyExtendedProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update singleValueLegacyExtendedProperty

Namespace: microsoft.graph

Update the properties of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

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
PATCH /me/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/contacts/{contactId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/mailFolders/{mailFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/contactFolders/{contactFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
PATCH /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_singlevaluelegacyextendedproperty"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
  "value": "Value value"
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
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
  "id": "47540889-0889-4754-8908-544789085447",
  "value": "Value value"
}
```

