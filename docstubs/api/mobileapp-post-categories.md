---
title: "Create categories"
description: "Create categories by posting to the categories collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create categories

Namespace: microsoft.graph

Create categories by posting to the categories collection.

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppCategory](../resources/mobileappcategory.md) object.

The following table shows the properties that are required when you create the [mobileAppCategory](../resources/mobileappcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name of the app category.|
|lastModifiedDateTime|DateTimeOffset|The date and time the mobileAppCategory was last modified.|



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/mobileappcategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileappcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps/{mobileAppId}/categories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileappcategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "68255c8f-5c8f-6825-8f5c-25688f5c2568",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00"
}
```

