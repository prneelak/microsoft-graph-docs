---
title: "Add deviceCompliancePolicySettingStateSummaries"
description: "Add deviceCompliancePolicySettingStateSummaries by posting to the deviceCompliancePolicySettingStateSummaries collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceCompliancePolicySettingStateSummaries

Namespace: microsoft.graph

Add deviceCompliancePolicySettingStateSummaries by posting to the deviceCompliancePolicySettingStateSummaries collection.

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
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|setting|String|The setting class name and property name.|
|settingName|String|Name of the setting.|
|platformType|Enumeration|Setting platform. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|unknownDeviceCount|Int32|Number of unknown devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|compliantDeviceCount|Int32|Number of compliant devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|errorDeviceCount|Int32|Number of error devices|
|conflictDeviceCount|Int32|Number of conflict devices|



## Response
If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancepolicysettingstatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "String",
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
  "@odata.type": "microsoft.graph.devicecompliancepolicysettingstatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "e2e47c44-7c44-e2e4-447c-e4e2447ce4e2",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "String",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

