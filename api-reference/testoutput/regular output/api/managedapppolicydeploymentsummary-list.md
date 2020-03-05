---
title: "List managedAppPolicyDeploymentSummaries"
description: "List properties and relationships of the managedAppPolicyDeploymentSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedAppPolicyDeploymentSummaries

Namespace: microsoft.graph

List properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) objects.

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
GET ** Collection URI for microsoft.graph.managedAppPolicyDeploymentSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicyDeploymentSummary](../resources/managedapppolicydeploymentsummary.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedapppolicydeploymentsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.managedAppPolicyDeploymentSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedapppolicydeploymentsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
      "id": "ca80d811-d811-ca80-11d8-80ca11d880ca",
      "displayName": "Display Name value",
      "configurationDeployedUserCount": 14,
      "lastRefreshTime": "2016-12-31T23:59:27.6543828+03:00",
      "configurationDeploymentSummaryPerApp": [
        {
          "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
          "mobileAppIdentifier": {
            "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
            "packageId": "Package Id value"
          },
          "configurationAppliedUserCount": 13
        }
      ],
      "version": "Version value"
    }
  ]
}
```

