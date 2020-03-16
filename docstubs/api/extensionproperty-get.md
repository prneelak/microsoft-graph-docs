---
title: "Get extensionProperty"
description: "Read properties and relationships of the extensionProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get extensionProperty

Namespace: microsoft.graph

Read properties and relationships of the [extensionProperty](../resources/extensionproperty.md) object.

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
GET /applications/{applicationsId}/extensionProperties/{extensionPropertyId}
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
If successful, this method returns a `200 OK` response code and [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_extensionproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}/extensionProperties/{extensionPropertyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": {
    "@odata.type": "#microsoft.graph.extensionProperty",
    "id": "8c26eb49-eb49-8c26-49eb-268c49eb268c",
    "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
    "appDisplayName": "App Display Name value",
    "name": "Name value",
    "dataType": "Data Type value",
    "isSyncedFromOnPremises": true,
    "targetObjects": [
      "Target Objects value"
    ]
  }
}
```

