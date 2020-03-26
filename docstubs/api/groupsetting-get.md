---
title: "Get groupSetting"
description: "Read properties and relationships of the groupSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupSetting

Namespace: microsoft.graph

Read properties and relationships of the [groupSetting](../resources/groupsetting.md) object.

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
GET /groupSettings/{groupSettingsId}
GET /groups/{groupsId}/settings/{groupSettingId}
GET /me/joinedTeams/{groupId}/settings/{groupSettingId}
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
If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/groupSettings/{groupSettingsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": {
    "@odata.type": "#microsoft.graph.groupSetting",
    "id": "a864431d-431d-a864-1d43-64a81d4364a8",
    "displayName": "Display Name value",
    "templateId": "Template Id value",
    "values": [
      {
        "@odata.type": "microsoft.graph.settingValue",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```

