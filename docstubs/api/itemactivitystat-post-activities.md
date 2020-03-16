---
title: "Create activities"
description: "Create activities by posting to the activities collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create activities

Namespace: microsoft.graph

Create activities by posting to the activities collection.

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
POST /me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [itemActivity](../resources/itemactivity.md) object.

The following table shows the properties that are required when you create the [itemActivity](../resources/itemactivity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|access|[accessAction](../resources/accessaction.md)||
|activityDateTime|DateTimeOffset||
|actor|[identitySet](../resources/identityset.md)||



## Response
If successful, this method returns a `201 Created` response code and a [itemActivity](../resources/itemactivity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemactivity_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/analytics/itemActivityStats/{itemActivityStatId}/activities
Content-type: application/json
Content-length: 550

{
  "@odata.type": "#microsoft.graph.itemActivity",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "2017-01-01T00:00:49.1508652+03:00",
  "actor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemactivity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 599

{
  "@odata.type": "#microsoft.graph.itemActivity",
  "id": "c2c24aa4-4aa4-c2c2-a44a-c2c2a44ac2c2",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "2017-01-01T00:00:49.1508652+03:00",
  "actor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

