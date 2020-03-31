---
title: "Update impossibleTravelRiskEvent"
description: "Update the properties of a impossibleTravelRiskEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update impossibleTravelRiskEvent

Namespace: microsoft.graph

Update the properties of a [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.

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
PATCH /impossibleTravelRiskEvents/{impossibleTravelRiskEventsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object.

The following table shows the properties that are required when you create the [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userDisplayName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userPrincipalName|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskEventType|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|riskLevel|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskEventStatus|Enumeration| Inherited from [identityRiskEvent](../resources/identityriskevent.md). Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|closedDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|createdDateTime|DateTimeOffset| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|userId|String| Inherited from [identityRiskEvent](../resources/identityriskevent.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|ipAddress|String| Inherited from [locatedRiskEvent](../resources/locatedriskevent.md)|
|userAgent|String||
|deviceInformation|String||
|isAtypicalLocation|Boolean||
|previousSigninDateTime|DateTimeOffset||
|previousLocation|[signInLocation](../resources/signinlocation.md)||
|previousIpAddress|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_impossibletravelriskevent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/impossibleTravelRiskEvents/{impossibleTravelRiskEventsId}
Content-type: application/json
Content-length: 1137

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2016-12-31T23:59:57.7568077+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:05.5928212+03:00",
  "userId": "User Id value",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "ipAddress": "Ip Address value",
  "userAgent": "User Agent value",
  "deviceInformation": "Device Information value",
  "isAtypicalLocation": true,
  "previousSigninDateTime": "2016-12-31T23:58:48.996189+03:00",
  "previousLocation": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "previousIpAddress": "Previous Ip Address value"
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
Content-Length: 1245

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "id": "be2ae172-e172-be2a-72e1-2abe72e12abe",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "riskEventDateTime": "2016-12-31T23:59:57.7568077+03:00",
  "riskEventType": "Risk Event Type value",
  "riskLevel": "String",
  "riskEventStatus": "String",
  "closedDateTime": "2017-01-01T00:01:05.5928212+03:00",
  "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
  "userId": "User Id value",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "ipAddress": "Ip Address value",
  "userAgent": "User Agent value",
  "deviceInformation": "Device Information value",
  "isAtypicalLocation": true,
  "previousSigninDateTime": "2016-12-31T23:58:48.996189+03:00",
  "previousLocation": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "previousIpAddress": "Previous Ip Address value"
}
```

