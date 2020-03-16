---
title: "List groupLifecyclePolicies"
description: "List properties and relationships of the groupLifecyclePolicy objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List groupLifecyclePolicies

Namespace: microsoft.graph

List properties and relationships of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects.

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
GET /groupLifecyclePolicies
GET /groups/{groupsId}/groupLifecyclePolicies
GET /me/joinedTeams/{groupId}/groupLifecyclePolicies
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
GET https://graph.microsoft.com/localtest/groupLifecyclePolicies
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
      "id": "77e566b0-66b0-77e5-b066-e577b066e577",
      "groupLifetimeInDays": 3,
      "managedGroupTypes": "Managed Group Types value",
      "alternateNotificationEmails": "Alternate Notification Emails value"
    }
  ]
}
```

