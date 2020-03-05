---
title: "List groupLifecyclePolicies"
description: "Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupLifecyclePolicies

Namespace: microsoft.graph

Get the groupLifecyclePolicies from the groupLifecyclePolicies navigation property.

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
GET /groups/{groupsId}/groupLifecyclePolicies
GET /me/joinedTeams/{groupId}/groupLifecyclePolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/groupLifecyclePolicies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.grouplifecyclepolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
      "id": "efd2c3af-c3af-efd2-afc3-d2efafc3d2ef",
      "groupLifetimeInDays": 3,
      "managedGroupTypes": "Managed Group Types value",
      "alternateNotificationEmails": "Alternate Notification Emails value"
    }
  ]
}
```

