---
title: "Add deviceEnrollmentConfigurations"
description: "Add deviceEnrollmentConfigurations by posting to the deviceEnrollmentConfigurations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceEnrollmentConfigurations

Namespace: microsoft.graph

Add deviceEnrollmentConfigurations by posting to the deviceEnrollmentConfigurations collection.

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
POST /deviceManagement/deviceEnrollmentConfigurations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|priority|Int32||
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|version|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceenrollmentconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceenrollmentconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 357

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "829fea57-ea57-829f-57ea-9f8257ea9f82",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "version": 7
}
```

