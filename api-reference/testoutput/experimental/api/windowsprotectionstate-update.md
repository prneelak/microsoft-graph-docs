---
title: "Update windowsProtectionState"
description: "Update the properties of a windowsProtectionState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsProtectionState

Namespace: microsoft.graph

Update the properties of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.

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
PATCH /me/managedDevices/{managedDeviceId}/windowsProtectionState
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsProtectionState](../resources/windowsprotectionstate.md) object.

The following table shows the properties that are required when you create the [windowsProtectionState](../resources/windowsprotectionstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|malwareProtectionEnabled|Boolean|Anti malware is enabled or not|
|deviceState|Enumeration|Computer's state (like clean or pending full scan or pending reboot etc). Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean|Real time protection is enabled or not?|
|networkInspectionSystemEnabled|Boolean|Network inspection system enabled or not?|
|quickScanOverdue|Boolean|Quick scan overdue or not?|
|fullScanOverdue|Boolean|Full scan overdue or not?|
|signatureUpdateOverdue|Boolean|Signature out of date or not?|
|rebootRequired|Boolean|Reboot required or not?|
|fullScanRequired|Boolean|Full scan required or not?|
|engineVersion|String|Current endpoint protection engine's version|
|signatureVersion|String|Current malware definitions version|
|antiMalwareVersion|String|Current anti malware version|
|lastQuickScanDateTime|DateTimeOffset|Last quick scan datetime|
|lastFullScanDateTime|DateTimeOffset|Last quick scan datetime|
|lastQuickScanSignatureVersion|String|Last quick scan signature version|
|lastFullScanSignatureVersion|String|Last full scan signature version|
|lastReportedDateTime|DateTimeOffset|Last device health status reported time|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/windowsprotectionstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsprotectionstate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/windowsProtectionState
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:41.0107406+03:00",
  "lastFullScanDateTime": "2016-12-31T23:57:54.954374+03:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2016-12-31T23:57:18.9477453+03:00"
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
Content-Length: 904

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "b90ddc2e-dc2e-b90d-2edc-0db92edc0db9",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:41.0107406+03:00",
  "lastFullScanDateTime": "2016-12-31T23:57:54.954374+03:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2016-12-31T23:57:18.9477453+03:00"
}
```

