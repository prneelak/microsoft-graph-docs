---
title: "List activities"
description: "Get the userActivities from the activities navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List activities

Namespace: microsoft.graph

Get the userActivities from the activities navigation property.

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
GET /me/activities
GET /users/{usersId}/activities
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
If successful, this method returns a `200 OK` response code and a collection of [userActivity](../resources/useractivity.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_useractivity"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/activities
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.useractivity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1435

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userActivity",
      "id": "7c2e5223-5223-7c2e-2352-2e7c23522e7c",
      "visualElements": {
        "@odata.type": "microsoft.graph.visualInfo",
        "attribution": {
          "@odata.type": "microsoft.graph.imageInfo",
          "iconUrl": "https://example.com/iconUrl/",
          "alternativeText": "Alternative Text value",
          "alternateText": "Alternate Text value",
          "addImageQuery": true
        },
        "backgroundColor": "Background Color value",
        "description": "Description value",
        "displayText": "Display Text value",
        "content": {
          "@odata.type": "microsoft.graph.Json"
        }
      },
      "activitySourceHost": "Activity Source Host value",
      "activationUrl": "https://example.com/activationUrl/",
      "appActivityId": "App Activity Id value",
      "appDisplayName": "App Display Name value",
      "contentUrl": "https://example.com/contentUrl/",
      "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
      "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
      "fallbackUrl": "https://example.com/fallbackUrl/",
      "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
      "userTimezone": "User Timezone value",
      "contentInfo": {
        "@odata.type": "microsoft.graph.Json"
      },
      "status": "String"
    }
  ]
}
```

