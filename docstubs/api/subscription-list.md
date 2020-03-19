---
title: "List subscriptions"
description: "List properties and relationships of the subscription objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List subscriptions

Namespace: microsoft.graph

List properties and relationships of the [subscription](../resources/subscription.md) objects.

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
GET /subscriptions
GET /workbooks/{workbooksId}/subscriptions
GET /me/drive/items/{driveItemId}/subscriptions
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
If successful, this method returns a `200 OK` response code and a collection of [subscription](../resources/subscription.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}
-->
``` http
GET https://graph.microsoft.com/localtest/subscriptions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.subscription)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 487

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.subscription",
      "id": "c461c987-c987-c461-87c9-61c487c961c4",
      "resource": "Resource value",
      "changeType": "Change Type value",
      "clientState": "Client State value",
      "notificationUrl": "https://example.com/notificationUrl/",
      "expirationDateTime": "2016-12-31T23:59:24.8520161+03:00",
      "applicationId": "Application Id value",
      "creatorId": "Creator Id value"
    }
  ]
}
```

