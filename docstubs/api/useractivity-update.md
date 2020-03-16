---
title: "Update userActivity"
description: "Update the properties of a userActivity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userActivity

Namespace: microsoft.graph

Update the properties of a [userActivity](../resources/useractivity.md) object.

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
PATCH /me/activities/{userActivityId}
PATCH /users/{usersId}/activities/{userActivityId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userActivity](../resources/useractivity.md) object.

The following table shows the properties that are required when you create the [userActivity](../resources/useractivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|visualElements|[visualInfo](../resources/visualinfo.md)||
|activitySourceHost|String||
|activationUrl|String||
|appActivityId|String||
|appDisplayName|String||
|contentUrl|String||
|createdDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|fallbackUrl|String||
|lastModifiedDateTime|DateTimeOffset||
|userTimezone|String||
|contentInfo|[Json](../resources/json.md)||
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_useractivity"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/activities/{userActivityId}
Content-type: application/json
Content-length: 1102

{
  "@odata.type": "#microsoft.graph.userActivity",
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
  "expirationDateTime": "2016-12-31T23:57:17.885665+03:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
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
Content-Length: 1274

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
```

