---
title: "List deviceManagementTroubleshootingEvents"
description: "Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementTroubleshootingEvents

Namespace: microsoft.graph

Get the deviceManagementTroubleshootingEvents from the deviceManagementTroubleshootingEvents navigation property.

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
GET /me/deviceManagementTroubleshootingEvents
GET /users/{usersId}/deviceManagementTroubleshootingEvents
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementtroubleshootingevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/deviceManagementTroubleshootingEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementtroubleshootingevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1037

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "0da8f15e-f15e-0da8-5ef1-a80d5ef1a80d",
      "eventDateTime": "2016-12-31T23:58:36.742225+00:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

