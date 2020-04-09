---
title: "Add activities"
description: "Add activities by posting to the activities collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add activities

Namespace: microsoft.graph

Add activities by posting to the activities collection.

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
POST /me/activities/$ref
POST /users/{usersId}/activities/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|status|Enumeration| Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_useractivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/activities
Content-type: application/json
Content-length: 1103

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
  "expirationDateTime": "2016-12-31T23:57:53.4850868+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.useractivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1275

{
  "@odata.type": "#microsoft.graph.userActivity",
  "id": "b6c0b87d-b87d-b6c0-7db8-c0b67db8c0b6",
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
  "createdDateTime": "2017-01-01T00:00:01.0610721+03:00",
  "expirationDateTime": "2016-12-31T23:57:53.4850868+03:00",
  "fallbackUrl": "https://example.com/fallbackUrl/",
  "lastModifiedDateTime": "2016-12-31T23:59:20.4130705+03:00",
  "userTimezone": "User Timezone value",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

