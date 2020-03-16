---
title: "Update groupLifecyclePolicy"
description: "Update the properties of a groupLifecyclePolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupLifecyclePolicy

Namespace: microsoft.graph

Update the properties of a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

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
PATCH /groupLifecyclePolicies/{groupLifecyclePoliciesId}
PATCH /groups/{groupsId}/groupLifecyclePolicies/{groupLifecyclePolicyId}
PATCH /me/joinedTeams/{groupId}/groupLifecyclePolicies/{groupLifecyclePolicyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

The following table shows the properties that are required when you create the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|groupLifetimeInDays|Int32||
|managedGroupTypes|String||
|alternateNotificationEmails|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/groupLifecyclePolicies/{groupLifecyclePoliciesId}
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "groupLifetimeInDays": 3,
  "managedGroupTypes": "Managed Group Types value",
  "alternateNotificationEmails": "Alternate Notification Emails value"
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
Content-Length: 266

{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "id": "87f7d5a2-d5a2-87f7-a2d5-f787a2d5f787",
  "groupLifetimeInDays": 3,
  "managedGroupTypes": "Managed Group Types value",
  "alternateNotificationEmails": "Alternate Notification Emails value"
}
```

