---
title: "Update restrictedSignIn"
description: "Update the properties of a restrictedSignIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update restrictedSignIn

Namespace: microsoft.graph

Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.

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
PATCH /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [restrictedSignIn](../resources/restrictedsignin.md) object.

The following table shows the properties that are required when you create the [restrictedSignIn](../resources/restrictedsignin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signin.md)|
|userDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/signin.md)|
|userId|String| Inherited from [signIn](../resources/signin.md)|
|appId|String| Inherited from [signIn](../resources/signin.md)|
|appDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|ipAddress|String| Inherited from [signIn](../resources/signin.md)|
|status|[signInStatus](../resources/signinstatus.md)| Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)| Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [signIn](../resources/signin.md)|
|correlationId|String| Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection| Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signin.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|resourceDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|resourceId|String| Inherited from [signIn](../resources/signin.md)|
|targetTenantId|Guid||



## Response
If successful, this method returns a `200 OK` response code and an updated [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_restrictedsignin"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/auditLogs/restrictedSignIns/{restrictedSignInId}
Content-type: application/json
Content-length: 2019

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
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
  "resourceId": "Resource Id value",
  "targetTenantId": "8a1cc620-c620-8a1c-20c6-1c8a20c61c8a"
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
Content-Length: 2127

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "c76f19e7-19e7-c76f-e719-6fc7e7196fc7",
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
  "resourceId": "Resource Id value",
  "targetTenantId": "8a1cc620-c620-8a1c-20c6-1c8a20c61c8a"
}
```

