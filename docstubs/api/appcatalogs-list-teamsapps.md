---
title: "List teamsApps"
description: "Get the teamsApps from the teamsApps navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsApps

Namespace: microsoft.graph

Get the teamsApps from the teamsApps navigation property.

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
GET /appCatalogs/teamsApps
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
If successful, this method returns a `200 OK` response code and a collection of [teamsApp](../resources/teamsapp.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsapp"
}
-->
``` http
GET https://graph.microsoft.com/localtest/appCatalogs/teamsApps
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsapp)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsApp",
      "id": "c7c9c3f2-c3f2-c7c9-f2c3-c9c7f2c3c9c7",
      "externalId": "External Id value",
      "displayName": "Display Name value",
      "distributionMethod": "String"
    }
  ]
}
```

