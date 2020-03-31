---
title: "Update directoryAudit"
description: "Update the properties of a directoryAudit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update directoryAudit

Namespace: microsoft.graph

Update the properties of a [directoryAudit](../resources/directoryaudit.md) object.

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
PATCH /auditLogs/directoryAudits/{directoryAuditId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [directoryAudit](../resources/directoryaudit.md) object.

The following table shows the properties that are required when you create the [directoryAudit](../resources/directoryaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|category|String||
|correlationId|String||
|result|Enumeration| Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.|
|resultReason|String||
|activityDisplayName|String||
|activityDateTime|DateTimeOffset||
|loggedByService|String||
|operationType|String||
|initiatedBy|[auditActivityInitiator](../resources/auditactivityinitiator.md)||
|targetResources|[targetResource](../resources/targetresource.md) collection||
|additionalDetails|[keyValue](../resources/keyvalue.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [directoryAudit](../resources/directoryaudit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directoryaudit"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/directoryAudits/{directoryAuditId}
Content-type: application/json
Content-length: 1484

{
  "@odata.type": "#microsoft.graph.directoryAudit",
  "category": "Category value",
  "correlationId": "Correlation Id value",
  "result": "String",
  "resultReason": "Result Reason value",
  "activityDisplayName": "Activity Display Name value",
  "activityDateTime": "2017-01-01T00:03:21.5368458+03:00",
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
Content-Length: 1533

{
  "@odata.type": "#microsoft.graph.directoryAudit",
  "id": "fc0aad9e-ad9e-fc0a-9ead-0afc9ead0afc",
  "category": "Category value",
  "correlationId": "Correlation Id value",
  "result": "String",
  "resultReason": "Result Reason value",
  "activityDisplayName": "Activity Display Name value",
  "activityDateTime": "2017-01-01T00:03:21.5368458+03:00",
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
```

