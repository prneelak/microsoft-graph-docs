---
title: "signIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signIn resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get signIn](../api/signin-get.md)|[signIn](../resources/signin.md)|Read properties and relationships of the [signIn](../resources/signin.md) object.|
|[Update signIn](../api/signin-update.md)|[signIn](../resources/signin.md)|Update the properties of a [signIn](../resources/signin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String||
|appId|String||
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection||
|clientAppUsed|String||
|conditionalAccessStatus|Enumeration|. Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String||
|createdDateTime|DateTimeOffset||
|deviceDetail|[deviceDetail](../resources/devicedetail.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String||
|isInteractive|Boolean||
|location|[signInLocation](../resources/signinlocation.md)||
|resourceDisplayName|String||
|resourceId|String||
|riskDetail|Enumeration|. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection||
|riskLevelAggregated|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration|. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](../resources/signinstatus.md)||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signIn",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appId": "String",
  "appDisplayName": "String",
  "ipAddress": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "clientAppUsed": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "correlationId": "String",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
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
  "resourceDisplayName": "String",
  "resourceId": "String"
}
```

