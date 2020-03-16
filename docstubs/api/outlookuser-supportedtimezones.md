---
title: "supportedTimeZones"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# supportedTimeZones

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
GET /me/outlook/supportedTimeZones
GET /users/{usersId}/outlook/supportedTimeZones
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|TimeZoneStandard|Enumeration||



## Response
If successful, this function returns a `200 OK` response code and a [timeZoneInformation](../resources/timezoneinformation.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "outlookuser_supportedtimezones"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/outlook/supportedTimeZones(TimeZoneStandard='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timezoneinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 97

{
  "value": [
    {
      "@odata.type": "microsoft.graph.timeZoneInformation"
    }
  ]
}
```

