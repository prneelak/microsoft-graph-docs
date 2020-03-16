---
title: "Update notificationMessageTemplate"
description: "Update the properties of a notificationMessageTemplate object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update notificationMessageTemplate

Namespace: microsoft.graph

Update the properties of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.

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
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.

The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/notificationmessagetemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Display name for the Notification Message Template.|
|defaultLocale|String|The default locale to fallback onto when the requested locale is not available.|
|brandingOptions|Enumeration|The Message Template Branding Options. Branding is defined in the Intune Admin Console. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_notificationmessagetemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
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
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "eb9f0d46-0d46-eb9f-460d-9feb460d9feb",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "String"
}
```

