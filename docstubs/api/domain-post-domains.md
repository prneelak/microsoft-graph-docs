---
title: "Create domain"
description: "Create a new domain object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domain

Namespace: microsoft.graph

Create a new [domain](../resources/domain.md) object.

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
POST /domains
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
|manufacturer|String||
|model|String||
|passwordNotificationWindowInDays|Int32||
|passwordValidityPeriodInDays|Int32||
|supportedServices|String collection||
|state|[domainState](../resources/domainstate.md)||



## Response
If successful, this method returns a `201 Created` response code and a [domain](../resources/domain.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domain_from_domains"
}
-->
``` http
POST https://graph.microsoft.com/localtest/domains
Content-type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.domain",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 733

{
  "@odata.type": "#microsoft.graph.domain",
  "id": "3374b703-b703-3374-03b7-743303b77433",
  "authenticationType": "Authentication Type value",
  "availabilityStatus": "Availability Status value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "passwordNotificationWindowInDays": 0,
  "passwordValidityPeriodInDays": 12,
  "supportedServices": [
    "Supported Services value"
  ],
  "state": {
    "@odata.type": "microsoft.graph.domainState",
    "status": "Status value",
    "operation": "Operation value",
    "lastActionDateTime": "2016-12-31T23:56:51.3643763+03:00"
  }
}
```

