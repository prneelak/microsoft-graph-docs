---
title: "Add deviceCompliancePolicies"
description: "Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceCompliancePolicies

Namespace: microsoft.graph

Add deviceCompliancePolicies by posting to the deviceCompliancePolicies collection.

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
POST /deviceManagement/deviceCompliancePolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicy](../resources/devicecompliancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Admin provided name of the device configuration.|
|version|Int32|Version of the device configuration.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicy](../resources/devicecompliancepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancepolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 160

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancepolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 332

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "c4fbfea9-fea9-c4fb-a9fe-fbc4a9fefbc4",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "displayName": "Display Name value",
  "version": 7
}
```

