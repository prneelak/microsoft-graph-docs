---
title: "Add userStatuses"
description: "Add userStatuses by posting to the userStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userStatuses

Namespace: microsoft.graph

Add userStatuses by posting to the userStatuses collection.

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String|User name of the DevicePolicyStatus.|
|devicesCount|Int32|Devices count for that user.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|userPrincipalName|String|UserPrincipalName.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationuserstatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 283

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:00:41.3711013+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationuserstatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 332

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "c6b0ea76-ea76-c6b0-76ea-b0c676eab0c6",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:00:41.3711013+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

