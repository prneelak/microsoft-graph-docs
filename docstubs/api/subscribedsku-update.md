---
title: "Update subscribedSku"
description: "Update the properties of a subscribedSku object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update subscribedSku

Namespace: microsoft.graph

Update the properties of a [subscribedSku](../resources/subscribedsku.md) object.

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
PATCH /subscribedSkus/{subscribedSkusId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [subscribedSku](../resources/subscribedsku.md) object.

The following table shows the properties that are required when you create the [subscribedSku](../resources/subscribedsku.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|capabilityStatus|String||
|consumedUnits|Int32||
|prepaidUnits|[licenseUnitsDetail](../resources/licenseunitsdetail.md)||
|servicePlans|[servicePlanInfo](../resources/serviceplaninfo.md) collection||
|skuId|Guid||
|skuPartNumber|String||
|appliesTo|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_subscribedsku"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/subscribedSkus/{subscribedSkusId}
Content-type: application/json
Content-length: 717

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "capabilityStatus": "Capability Status value",
  "consumedUnits": 13,
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail",
    "enabled": 7,
    "suspended": 9,
    "warning": 7
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "06018a28-8a28-0601-288a-0106288a0106",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "bbef9239-9239-bbef-3992-efbb3992efbb",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
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
Content-Length: 766

{
  "@odata.type": "#microsoft.graph.subscribedSku",
  "id": "0309ad56-ad56-0309-56ad-090356ad0903",
  "capabilityStatus": "Capability Status value",
  "consumedUnits": 13,
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail",
    "enabled": 7,
    "suspended": 9,
    "warning": 7
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo",
      "servicePlanId": "06018a28-8a28-0601-288a-0106288a0106",
      "servicePlanName": "Service Plan Name value",
      "provisioningStatus": "Provisioning Status value",
      "appliesTo": "Applies To value"
    }
  ],
  "skuId": "bbef9239-9239-bbef-3992-efbb3992efbb",
  "skuPartNumber": "Sku Part Number value",
  "appliesTo": "Applies To value"
}
```

