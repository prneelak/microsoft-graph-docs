---
title: "Add deviceConfigurationConflictSummary"
description: "Add deviceConfigurationConflictSummary by posting to the deviceConfigurationConflictSummary collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceConfigurationConflictSummary

Namespace: microsoft.graph

Add deviceConfigurationConflictSummary by posting to the deviceConfigurationConflictSummary collection.

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
POST /deviceManagement/deviceConfigurationConflictSummary/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|conflictingDeviceConfigurations|[settingSource](../resources/settingsource.md) collection|The set of policies in conflict with the given setting|
|contributingSettings|String collection|The set of settings in conflict with the given policies|
|deviceCheckinsImpacted|Int32|The count of checkins impacted by the conflicting policies and settings|



## Response
If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/deviceconfigurationconflictsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationconflictsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationconflictsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "id": "3d2b7f41-7f41-3d2b-417f-2b3d417f2b3d",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

