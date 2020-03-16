---
title: "Update deviceComplianceScheduledActionForRule"
description: "Update the properties of a deviceComplianceScheduledActionForRule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceComplianceScheduledActionForRule

Namespace: microsoft.graph

Update the properties of a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.

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
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.

The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|ruleName|String|Name of the rule which this scheduled action applies to.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancescheduledactionforrule"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
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
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "681c282d-282d-681c-2d28-1c682d281c68",
  "ruleName": "Rule Name value"
}
```

