---
title: "restrictedSignIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# restrictedSignIn resource type


Namespace: microsoft.graph




Inherits from [signIn](../resources/signin.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get restrictedSignIn](../api/restrictedsignin-get.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Read properties and relationships of the [restrictedSignIn](../resources/restrictedsignin.md) object.|
|[Update restrictedSignIn](../api/restrictedsignin-update.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String| Inherited from [signIn](../resources/signin.md)|
|appDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|appId|String| Inherited from [signIn](../resources/signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationMethodsUsed|String collection| Inherited from [signIn](../resources/signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection| Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String| Inherited from [signIn](../resources/signin.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)| Inherited from [signIn](../resources/signin.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [signIn](../resources/signin.md)|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)| Inherited from [signIn](../resources/signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection| Inherited from [signIn](../resources/signin.md)|
|originalRequestId|String| Inherited from [signIn](../resources/signin.md)|
|processingTimeInMilliseconds|Int32| Inherited from [signIn](../resources/signin.md)|
|resourceDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|resourceId|String| Inherited from [signIn](../resources/signin.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signin.md)|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String| Inherited from [signIn](../resources/signin.md)|
|servicePrincipalName|String| Inherited from [signIn](../resources/signin.md)|
|status|[signInStatus](../resources/signinstatus.md)| Inherited from [signIn](../resources/signin.md)|
|targetTenantId|Guid||
|tokenIssuerName|String| Inherited from [signIn](../resources/signin.md)|
|tokenIssuerType|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String| Inherited from [signIn](../resources/signin.md)|
|userDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|userId|String| Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/signin.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedSignIn",
  "baseType": "microsoft.graph.signIn",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "String (identifier)",
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "isInteractive": true,
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": 1024,
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "targetTenantId": "Guid"
}
```

