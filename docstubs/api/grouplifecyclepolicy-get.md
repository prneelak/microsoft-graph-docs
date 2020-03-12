---
title: "Get groupLifecyclePolicy"
description: "Read properties and relationships of the groupLifecyclePolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupLifecyclePolicy

Namespace: microsoft.graph

Read properties and relationships of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

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
GET /groupLifecyclePolicies/{groupLifecyclePoliciesId}
GET /groups/{groupsId}/groupLifecyclePolicies/{groupLifecyclePolicyId}
GET /me/joinedTeams/{groupId}/groupLifecyclePolicies/{groupLifecyclePolicyId}
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
If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groupLifecyclePolicies/{groupLifecyclePoliciesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": {
    "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
    "id": "f3261e08-1e08-f326-081e-26f3081e26f3",
    "groupLifetimeInDays": 3,
    "managedGroupTypes": "Managed Group Types value",
    "alternateNotificationEmails": "Alternate Notification Emails value"
  }
}
```

