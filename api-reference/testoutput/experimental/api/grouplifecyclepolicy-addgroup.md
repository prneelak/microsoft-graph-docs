---
title: "addGroup"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# addGroup

Namespace: microsoft.graph



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
POST /groupLifecyclePolicies/{groupLifecyclePoliciesId}/addGroup
POST /groups/{groupsId}/groupLifecyclePolicies/{groupLifecyclePolicyId}/addGroup
POST /me/joinedGroups/{groupId}/groupLifecyclePolicies/{groupLifecyclePolicyId}/addGroup
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|groupId|String||



## Response
If successful, this action returns a `200 OK` response code and a Boolean in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_addgroup"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groupLifecyclePolicies/{groupLifecyclePoliciesId}/addGroup

Content-type: application/json
Content-length: 35

{
  "groupId": "Group Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "edm.boolean"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```

