---
title: "Update deviceAppManagement"
description: "Update the properties of a deviceAppManagement object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceAppManagement

Namespace: microsoft.graph

Update the properties of a [deviceAppManagement](../resources/deviceappmanagement.md) object.

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
PATCH /deviceAppManagement
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceAppManagement](../resources/deviceappmanagement.md) object.

The following table shows the properties that are required when you create the [deviceAppManagement](../resources/deviceappmanagement.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|The last time the apps from the Microsoft Store for Business were synced successfully for the account.|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Whether the account is enabled for syncing applications from the Microsoft Store for Business.|
|microsoftStoreForBusinessLanguage|String|The locale information used to sync applications from the Microsoft Store for Business. Cultures that are specific to a country/region. The names of these cultures follow RFC 4646 (Windows Vista and later). The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166. For example, en-US for English (United States) is a specific culture.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|The last time an application sync from the Microsoft Store for Business was completed.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/deviceappmanagement.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceappmanagement"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceAppManagement
Content-type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:58:19.9096006+03:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:01:22.7952571+03:00"
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
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "e894643d-643d-e894-3d64-94e83d6494e8",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:58:19.9096006+03:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:01:22.7952571+03:00"
}
```

