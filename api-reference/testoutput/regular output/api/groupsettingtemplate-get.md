---
title: "Get groupSettingTemplate"
description: "Read properties and relationships of the groupSettingTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get groupSettingTemplate

Namespace: microsoft.graph

Read properties and relationships of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object.

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
GET /groupSettingTemplates/{groupSettingTemplatesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groupSettingTemplates/{groupSettingTemplatesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.groupSettingTemplate",
    "id": "e7de2e03-2e03-e7de-032e-dee7032edee7",
    "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "values": [
      {
        "@odata.type": "microsoft.graph.settingTemplateValue",
        "name": "Name value",
        "type": "Type value",
        "defaultValue": "Default Value value"
      }
    ]
  }
}
```

