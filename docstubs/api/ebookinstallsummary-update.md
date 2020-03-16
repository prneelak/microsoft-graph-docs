---
title: "Update eBookInstallSummary"
description: "Update the properties of a eBookInstallSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update eBookInstallSummary

Namespace: microsoft.graph

Update the properties of a [eBookInstallSummary](../resources/ebookinstallsummary.md) object.

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
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.

The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/ebookinstallsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Number of Devices that have successfully installed this book.|
|failedDeviceCount|Int32|Number of Devices that have failed to install this book.|
|notInstalledDeviceCount|Int32|Number of Devices that does not have this book installed.|
|installedUserCount|Int32|Number of Users whose devices have all succeeded to install this book.|
|failedUserCount|Int32|Number of Users that have 1 or more device that failed to install this book.|
|notInstalledUserCount|Int32|Number of Users that did not install this book.|



## Response
If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/ebookinstallsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_ebookinstallsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
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
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "78f9688d-688d-78f9-8d68-f9788d68f978",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

