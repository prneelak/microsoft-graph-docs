---
title: "Update onPremisesConditionalAccessSettings"
description: "Update the properties of a onPremisesConditionalAccessSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onPremisesConditionalAccessSettings

Namespace: microsoft.graph

Update the properties of a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

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
PATCH /deviceManagement/conditionalAccessSettings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.

The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|enabled|Boolean|Indicates if on premises conditional access is enabled for this organization|
|includedGroups|Guid collection|User groups that will be targeted by on premises conditional access. All users in these groups will be required to have mobile device managed and compliant for mail access.|
|excludedGroups|Guid collection|User groups that will be exempt by on premises conditional access. All users in these groups will be exempt from the conditional access policy.|
|overrideDefaultRule|Boolean|Override the default access rule when allowing a device to ensure access is granted.|



## Response
If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onpremisesconditionalaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "deaf509d-509d-deaf-9d50-afde9d50afde"
  ],
  "excludedGroups": [
    "46651d13-1d13-4665-131d-6546131d6546"
  ],
  "overrideDefaultRule": true
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
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "e7cedb6a-db6a-e7ce-6adb-cee76adbcee7",
  "enabled": true,
  "includedGroups": [
    "deaf509d-509d-deaf-9d50-afde9d50afde"
  ],
  "excludedGroups": [
    "46651d13-1d13-4665-131d-6546131d6546"
  ],
  "overrideDefaultRule": true
}
```

