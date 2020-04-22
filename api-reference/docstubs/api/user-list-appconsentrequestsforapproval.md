---
title: "List appConsentRequestsForApproval"
description: "Get the appConsentRequests from the appConsentRequestsForApproval navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List appConsentRequestsForApproval

Namespace: microsoft.graph

Get the appConsentRequests from the appConsentRequestsForApproval navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/appConsentRequestsForApproval
GET /users/{usersId}/appConsentRequestsForApproval
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/appConsentRequestsForApproval
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.appconsentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appConsentRequest",
      "id": "fe27a918-a918-fe27-18a9-27fe18a927fe",
      "appId": "App Id value",
      "appDisplayName": "App Display Name value",
      "consentType": "Consent Type value",
      "pendingScopes": [
        {
          "@odata.type": "microsoft.graph.appConsentRequestScope",
          "displayName": "Display Name value"
        }
      ]
    }
  ]
}
```

