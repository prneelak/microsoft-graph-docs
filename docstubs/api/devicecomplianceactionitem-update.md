---
title: "Update deviceComplianceActionItem"
description: "Update the properties of a deviceComplianceActionItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceComplianceActionItem

Namespace: microsoft.graph

Update the properties of a [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.

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
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object.

The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|gracePeriodHours|Int32|Number of hours to wait till the action will be enforced. Valid values 0 to 8760|
|actionType|Enumeration|What action to take. Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.|
|notificationTemplateId|String|What notification Message template to use|
|notificationMessageCCList|String collection|A list of group IDs to speicify who to CC this notification message to.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/devicecomplianceactionitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicecomplianceactionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "String",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
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
Content-Length: 314

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "34dd142b-142b-34dd-2b14-dd342b14dd34",
  "gracePeriodHours": 0,
  "actionType": "String",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

