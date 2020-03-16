---
title: "Add deviceSettingStateSummaries"
description: "Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceSettingStateSummaries

Namespace: microsoft.graph

Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.

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
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.

The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/settingstatedevicesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingName|String|Name of the setting|
|instancePath|String|Name of the InstancePath for the setting|
|unknownDeviceCount|Int32|Device Unkown count for the setting|
|notApplicableDeviceCount|Int32|Device Not Applicable count for the setting|
|compliantDeviceCount|Int32|Device Compliant count for the setting|
|remediatedDeviceCount|Int32|Device Compliant count for the setting|
|nonCompliantDeviceCount|Int32|Device NonCompliant count for the setting|
|errorDeviceCount|Int32|Device error count for the setting|
|conflictDeviceCount|Int32|Device conflict error count for the setting|



## Response
If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_settingstatedevicesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.settingstatedevicesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "b3cc6db0-6db0-b3cc-b06d-ccb3b06dccb3",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

