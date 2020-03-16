---
title: "Add exchangeConnectors"
description: "Add exchangeConnectors by posting to the exchangeConnectors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add exchangeConnectors

Namespace: microsoft.graph

Add exchangeConnectors by posting to the exchangeConnectors collection.

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
POST /deviceManagement/exchangeConnectors/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object.

The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last sync time for the Exchange Connector|
|status|Enumeration|Exchange Connector Status. Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|Email address used to configure the Service To Service Exchange Connector.|
|serverName|String|The name of the Exchange server.|
|connectorServerName|String|The name of the server hosting the Exchange Connector.|
|exchangeConnectorType|Enumeration|The type of Exchange Connector Configured. Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|String|The version of the ExchangeConnectorAgent|
|exchangeAlias|String|An alias assigned to the Exchange server|
|exchangeOrganization|String|Exchange Organization to the Exchange server|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/devicemanagementexchangeconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementexchangeconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:00:47.2519883+03:00",
  "status": "String",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "String",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementexchangeconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "66217a06-7a06-6621-067a-2166067a2166",
  "lastSyncDateTime": "2017-01-01T00:00:47.2519883+03:00",
  "status": "String",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "String",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

