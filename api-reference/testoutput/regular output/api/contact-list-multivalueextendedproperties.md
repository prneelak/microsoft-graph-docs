---
title: "List multiValueExtendedProperties"
description: "Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List multiValueExtendedProperties

Namespace: microsoft.graph

Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.

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
GET /me/contacts/{contactId}/multiValueExtendedProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_multivaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/contacts/{contactId}/multiValueExtendedProperties
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.multivaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
      "id": "ff81e7e1-e7e1-ff81-e1e7-81ffe1e781ff",
      "value": [
        "Value value"
      ]
    }
  ]
}
```

