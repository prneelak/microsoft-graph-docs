---
title: "Update applePushNotificationCertificate"
description: "Update the properties of a applePushNotificationCertificate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update applePushNotificationCertificate

Namespace: microsoft.graph

Update the properties of a [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

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
PATCH /deviceManagement/applePushNotificationCertificate
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.

The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appleIdentifier|String|Apple Id of the account used to create the MDM push certificate.|
|topicIdentifier|String|Topic Id.|
|lastModifiedDateTime|DateTimeOffset|Last modified date and time for Apple push notification certificate.|
|expirationDateTime|DateTimeOffset|The expiration date and time for Apple push notification certificate.|
|certificate|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_applepushnotificationcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "expirationDateTime": "2016-12-31T23:59:11.273206+03:00",
  "certificate": "Certificate value"
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
Content-Length: 381

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "76b44430-4430-76b4-3044-b4763044b476",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "expirationDateTime": "2016-12-31T23:59:11.273206+03:00",
  "certificate": "Certificate value"
}
```

