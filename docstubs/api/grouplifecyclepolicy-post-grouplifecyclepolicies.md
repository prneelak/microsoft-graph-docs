---
title: "Create groupLifecyclePolicy"
description: "Create a new groupLifecyclePolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create groupLifecyclePolicy

Namespace: microsoft.graph

Create a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

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
POST /groupLifecyclePolicies
POST /groups/{groupsId}/groupLifecyclePolicies
POST /me/joinedTeams/{groupId}/groupLifecyclePolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_grouplifecyclepolicies"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groupLifecyclePolicies
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
  "truncated": true,
  "@odata.type": "microsoft.graph.grouplifecyclepolicy"
}
-->
``` http
HTTP/1.1 201 Created
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

