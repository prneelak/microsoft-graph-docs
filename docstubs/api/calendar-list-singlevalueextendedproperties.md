---
title: "List singleValueExtendedProperties"
description: "Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List singleValueExtendedProperties

Namespace: microsoft.graph

Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
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
GET ** Collection URI for microsoft.graph.singleValueLegacyExtendedProperty not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.singleValueLegacyExtendedProperty not found
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.singlevaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
      "id": "2d92d3bb-d3bb-2d92-bbd3-922dbbd3922d",
      "value": "Value value"
    }
  ]
}
```

