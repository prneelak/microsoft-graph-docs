---
title: "recent"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# recent

Namespace: microsoft.graph



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
GET /me/activities/recent
GET /users/{usersId}/activities/recent
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [userActivity](../resources/useractivity.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "useractivity_recent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/activities/recent
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
Content-Length: 919

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userActivity",
      "id": "7c2e5223-5223-7c2e-2352-2e7c23522e7c",
      "visualElements": {
        "@odata.type": "microsoft.graph.visualInfo"
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

