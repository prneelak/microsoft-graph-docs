---
title: "Update groupSetting"
description: "Update the properties of a groupSetting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update groupSetting

Namespace: microsoft.graph

Update the properties of a [groupSetting](../resources/groupsetting.md) object.

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
PATCH /groupSettings/{groupSettingsId}
PATCH /groups/{groupsId}/settings/{groupSettingId}
PATCH /me/joinedTeams/{groupId}/settings/{groupSettingId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [groupSetting](../resources/groupsetting.md) object.

The following table shows the properties that are required when you create the [groupSetting](../resources/groupsetting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|templateId|String||
|values|[settingValue](../resources/settingvalue.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [groupSetting](../resources/groupsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/groupSettings/{groupSettingsId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.groupSetting",
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
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.groupSetting",
  "id": "264a23e5-23e5-264a-e523-4a26e5234a26",
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
```

