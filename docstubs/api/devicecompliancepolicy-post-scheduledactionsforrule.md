---
title: "Add scheduledActionsForRule"
description: "Add scheduledActionsForRule by posting to the scheduledActionsForRule collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add scheduledActionsForRule

Namespace: microsoft.graph

Add scheduledActionsForRule by posting to the scheduledActionsForRule collection.

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
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object.

The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|ruleName|String|Name of the rule which this scheduled action applies to.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/devicecompliancescheduledactionforrule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancescheduledactionforrule_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancescheduledactionforrule"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "681c282d-282d-681c-2d28-1c682d281c68",
  "ruleName": "Rule Name value"
}
```

