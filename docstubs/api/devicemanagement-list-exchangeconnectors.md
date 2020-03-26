---
title: "List exchangeConnectors"
description: "Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List exchangeConnectors

Namespace: microsoft.graph

Get the deviceManagementExchangeConnectors from the exchangeConnectors navigation property.

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
GET /deviceManagement/exchangeConnectors
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
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementexchangeconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementexchangeconnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 605

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "c04a1fc9-1fc9-c04a-c91f-4ac0c91f4ac0",
      "lastSyncDateTime": "2016-12-31T23:59:10.2626583+03:00",
      "status": "String",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "String",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```

