---
title: "List extensionProperties"
description: "Get the extensionProperties from the extensionProperties navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List extensionProperties

Namespace: microsoft.graph

Get the extensionProperties from the extensionProperties navigation property.

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
GET /applications/{applicationsId}/extensionProperties
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_extensionproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/extensionProperties
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extensionproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extensionProperty",
      "id": "4383875c-875c-4383-5c87-83435c878343",
      "deletedDateTime": "2017-01-01T00:00:42.0561578+03:00",
      "appDisplayName": "App Display Name value",
      "name": "Name value",
      "dataType": "Data Type value",
      "isSyncedFromOnPremises": true,
      "targetObjects": [
        "Target Objects value"
      ]
    }
  ]
}
```

