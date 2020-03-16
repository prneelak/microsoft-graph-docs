---
title: "List directoryAudits"
description: "Get the directoryAudits from the directoryAudits navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List directoryAudits

Namespace: microsoft.graph

Get the directoryAudits from the directoryAudits navigation property.

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
GET /auditLogs/directoryAudits
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
If successful, this method returns a `200 OK` response code and a collection of [directoryAudit](../resources/directoryaudit.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/directoryAudits
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.directoryaudit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1754

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.directoryAudit",
      "id": "cf0550c9-50c9-cf05-c950-05cfc95005cf",
      "category": "Category value",
      "correlationId": "Correlation Id value",
      "result": "String",
      "resultReason": "Result Reason value",
      "activityDisplayName": "Activity Display Name value",
      "activityDateTime": "2017-01-01T00:00:49.1508652+03:00",
      "loggedByService": "Logged By Service value",
      "operationType": "Operation Type value",
      "initiatedBy": {
        "@odata.type": "microsoft.graph.auditActivityInitiator",
        "user": {
          "@odata.type": "microsoft.graph.userIdentity",
          "id": "Id value",
          "displayName": "Display Name value",
          "ipAddress": "Ip Address value",
          "userPrincipalName": "User Principal Name value"
        },
        "app": {
          "@odata.type": "microsoft.graph.appIdentity",
          "appId": "App Id value",
          "servicePrincipalId": "Service Principal Id value",
          "servicePrincipalName": "Service Principal Name value"
        }
      },
      "targetResources": [
        {
          "@odata.type": "microsoft.graph.targetResource",
          "type": "Type value",
          "groupType": "String",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.modifiedProperty",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ]
        }
      ],
      "additionalDetails": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

