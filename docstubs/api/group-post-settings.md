---
title: "Add settings"
description: "Add settings by posting to the settings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add settings

Namespace: microsoft.graph

Add settings by posting to the settings collection.

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
POST /groups/{groupsId}/settings/$ref
POST /me/joinedTeams/{groupId}/settings/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [groupSetting](../resources/groupsetting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/settings
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
  "truncated": true,
  "@odata.type": "microsoft.graph.groupsetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.groupSetting",
  "id": "a650a5f7-a5f7-a650-f7a5-50a6f7a550a6",
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

