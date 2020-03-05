---
title: "Get applePushNotificationCertificate"
description: "Read properties and relationships of the applePushNotificationCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get applePushNotificationCertificate

Namespace: microsoft.graph

Read properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

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
GET /deviceManagement/applePushNotificationCertificate
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_applepushnotificationcertificate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/applePushNotificationCertificate
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
    "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
    "id": "76b44430-4430-76b4-3044-b4763044b476",
    "appleIdentifier": "Apple Identifier value",
    "topicIdentifier": "Topic Identifier value",
    "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
    "expirationDateTime": "2016-12-31T23:59:11.273206+03:00",
    "certificate": "Certificate value"
  }
}
```

