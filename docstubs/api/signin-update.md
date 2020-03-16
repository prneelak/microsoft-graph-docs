---
title: "Update signIn"
description: "Update the properties of a signIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update signIn

Namespace: microsoft.graph

Update the properties of a [signIn](../resources/signin.md) object.

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
PATCH /auditLogs/signIns/{signInId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [signIn](../resources/signin.md) object.

The following table shows the properties that are required when you create the [signIn](../resources/signin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|userDisplayName|String||
|userPrincipalName|String||
|userId|String||
|appId|String||
|appDisplayName|String||
|ipAddress|String||
|status|[signInStatus](../resources/signinstatus.md)||
|clientAppUsed|String||
|deviceDetail|[deviceDetail](../resources/devicedetail.md)||
|location|[signInLocation](../resources/signinlocation.md)||
|correlationId|String||
|conditionalAccessStatus|Enumeration|. Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection||
|isInteractive|Boolean||
|riskDetail|Enumeration|. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLevelAggregated|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration|. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection|. Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|resourceDisplayName|String||
|resourceId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [signIn](../resources/signin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_signin"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/auditLogs/signIns/{signInId}
Content-type: application/json
Content-length: 1948

{
  "@odata.type": "#microsoft.graph.signIn",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "ipAddress": "Ip Address value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "clientAppUsed": "Client App Used value",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
    "deviceId": "Device Id value",
    "displayName": "Display Name value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
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
  "correlationId": "Correlation Id value",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
      "id": "Id value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "result": "String"
    }
  ],
  "isInteractive": true,
  "riskDetail": "String",
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "riskEventTypes": [
    "String"
  ],
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value"
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
Content-Length: 2056

{
  "@odata.type": "#microsoft.graph.signIn",
  "id": "490cd306-d306-490c-06d3-0c4906d30c49",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "userId": "User Id value",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "ipAddress": "Ip Address value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "clientAppUsed": "Client App Used value",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
    "deviceId": "Device Id value",
    "displayName": "Display Name value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
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
  "correlationId": "Correlation Id value",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
      "id": "Id value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "result": "String"
    }
  ],
  "isInteractive": true,
  "riskDetail": "String",
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "riskEventTypes": [
    "String"
  ],
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value"
}
```

