---
title: "Update domain"
description: "Update the properties of a domain object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domain

Namespace: microsoft.graph

Update the properties of a [domain](../resources/domain.md) object.

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
PATCH /domains/{domainsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [domain](../resources/domain.md) object.

The following table shows the properties that are required when you create the [domain](../resources/domain.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|authenticationType|String||
|availabilityStatus|String||
|isAdminManaged|Boolean||
|isDefault|Boolean||
|isInitial|Boolean||
|isRoot|Boolean||
|isVerified|Boolean||
|passwordNotificationWindowInDays|Int32||
|passwordValidityPeriodInDays|Int32||
|supportedServices|String collection||
|state|[domainState](../resources/domainstate.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [domain](../resources/domain.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domain"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domains/{domainsId}
Content-type: application/json
Content-length: 616

{
  "@odata.type": "#microsoft.graph.domain",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00"
  }
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
Content-Length: 665

{
  "@odata.type": "#microsoft.graph.domain",
  "id": "da19e1d0-e1d0-da19-d0e1-19dad0e119da",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2016-12-31T23:59:45.6080321+03:00"
  }
}
```

