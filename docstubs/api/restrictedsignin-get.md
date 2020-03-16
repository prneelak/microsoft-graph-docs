---
title: "Get restrictedSignIn"
description: "Read properties and relationships of the restrictedSignIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get restrictedSignIn

Namespace: microsoft.graph

Read properties and relationships of the [restrictedSignIn](../resources/restrictedsignin.md) object.

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
GET /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/restrictedSignIns/{restrictedSignInId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedSignIn"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2274

{
  "value": {
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
}
```

