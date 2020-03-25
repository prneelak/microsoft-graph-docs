---
title: "Get deviceAppManagement"
description: "Read properties and relationships of the deviceAppManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceAppManagement

Namespace: microsoft.graph

Read properties and relationships of the [deviceAppManagement](../resources/deviceappmanagement.md) object.

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
GET /deviceAppManagement
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/deviceappmanagement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceappmanagement"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "64431897-1897-6443-9718-436497184364",
    "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:47.8483628+03:00",
    "isEnabledForMicrosoftStoreForBusiness": true,
    "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
    "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:31.6714342+03:00"
  }
}
```

