---
title: "List alerts"
description: "Get the alerts from the alerts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List alerts

Namespace: microsoft.graph

Get the alerts from the alerts navigation property.

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
GET /Security/alerts
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
If successful, this method returns a `200 OK` response code and a collection of [alert](../resources/alert.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_alert"
}
-->
``` http
GET https://graph.microsoft.com/beta/Security/alerts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.alert)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6086

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.alert",
      "id": "0a1e0bc9-0bc9-0a1e-c90b-1e0ac90b1e0a",
      "activityGroupName": "Activity Group Name value",
      "assignedTo": "Assigned To value",
      "azureSubscriptionId": "Azure Subscription Id value",
      "azureTenantId": "Azure Tenant Id value",
      "category": "Category value",
      "closedDateTime": "2016-12-31T23:59:08.0305042+03:00",
      "cloudAppStates": [
        {
          "@odata.type": "microsoft.graph.cloudAppSecurityState",
          "destinationServiceIp": "Destination Service Ip value",
          "destinationServiceName": "Destination Service Name value",
          "riskScore": "Risk Score value"
        }
      ],
      "comments": [
        "Comments value"
      ],
      "confidence": 10,
      "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
      "description": "Description value",
      "detectionIds": [
        "Detection Ids value"
      ],
      "eventDateTime": "2016-12-31T23:58:48.6358831+03:00",
      "feedback": "String",
      "fileStates": [
        {
          "@odata.type": "microsoft.graph.fileSecurityState",
          "fileHash": {
            "@odata.type": "microsoft.graph.fileHash",
            "hashType": "String",
            "hashValue": "Hash Value value"
          },
          "name": "Name value",
          "path": "Path value"
        }
      ],
      "historyStates": [
        {
          "@odata.type": "microsoft.graph.alertHistoryState",
          "appId": "App Id value",
          "status": "String",
          "updatedDateTime": "2017-01-01T00:02:18.8023442+03:00",
          "user": "User value"
        }
      ],
      "hostStates": [
        {
          "@odata.type": "microsoft.graph.hostSecurityState",
          "fqdn": "Fqdn value",
          "isAzureAdJoined": true,
          "isAzureAdRegistered": true,
          "isHybridAzureDomainJoined": true,
          "netBiosName": "Net Bios Name value",
          "os": "Os value",
          "privateIpAddress": "Private Ip Address value",
          "publicIpAddress": "Public Ip Address value"
        }
      ],
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
      "malwareStates": [
        {
          "@odata.type": "microsoft.graph.malwareState",
          "family": "Family value",
          "severity": "Severity value",
          "wasRunning": true
        }
      ],
      "networkConnections": [
        {
          "@odata.type": "microsoft.graph.networkConnection",
          "applicationName": "Application Name value",
          "destinationAddress": "Destination Address value",
          "destinationDomain": "Destination Domain value",
          "destinationPort": "Destination Port value",
          "destinationUrl": "https://example.com/destinationUrl/",
          "direction": "String",
          "domainRegisteredDateTime": "2017-01-01T00:00:50.5192754+03:00",
          "localDnsName": "Local Dns Name value",
          "natDestinationAddress": "Nat Destination Address value",
          "natDestinationPort": "Nat Destination Port value",
          "natSourceAddress": "Nat Source Address value",
          "natSourcePort": "Nat Source Port value",
          "protocol": "String",
          "sourceAddress": "Source Address value",
          "sourcePort": "Source Port value",
          "status": "String",
          "urlParameters": "Url Parameters value"
        }
      ],
      "processes": [
        {
          "@odata.type": "microsoft.graph.process",
          "accountName": "Account Name value",
          "commandLine": "Command Line value",
          "integrityLevel": "String",
          "isElevated": true,
          "parentProcessCreatedDateTime": "2016-12-31T23:57:21.3479752+03:00",
          "parentProcessId": 15,
          "parentProcessName": "Parent Process Name value",
          "processId": 9
        }
      ],
      "recommendedActions": [
        "Recommended Actions value"
      ],
      "registryKeyStates": [
        {
          "@odata.type": "microsoft.graph.registryKeyState",
          "hive": "String",
          "key": "Key value",
          "oldKey": "Old Key value",
          "oldValueData": "Old Value Data value",
          "oldValueName": "Old Value Name value",
          "operation": "String",
          "valueData": "Value Data value",
          "valueName": "Value Name value",
          "valueType": "String"
        }
      ],
      "severity": "String",
      "sourceMaterials": [
        "Source Materials value"
      ],
      "status": "String",
      "tags": [
        "Tags value"
      ],
      "title": "Title value",
      "triggers": [
        {
          "@odata.type": "microsoft.graph.alertTrigger",
          "type": "Type value",
          "value": "Value value"
        }
      ],
      "userStates": [
        {
          "@odata.type": "microsoft.graph.userSecurityState",
          "aadUserId": "Aad User Id value",
          "domainName": "Domain Name value",
          "emailRole": "String",
          "isVpn": true,
          "logonDateTime": "2017-01-01T00:01:44.5346112+03:00",
          "logonId": "Logon Id value",
          "logonIp": "Logon Ip value",
          "logonLocation": "Logon Location value",
          "logonType": "String",
          "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
          "userAccountType": "String",
          "userPrincipalName": "User Principal Name value"
        }
      ],
      "vendorInformation": {
        "@odata.type": "microsoft.graph.securityVendorInformation",
        "provider": "Provider value",
        "providerVersion": "Provider Version value",
        "subProvider": "Sub Provider value",
        "vendor": "Vendor value"
      },
      "vulnerabilityStates": [
        {
          "@odata.type": "microsoft.graph.vulnerabilityState",
          "cve": "Cve value"
        }
      ]
    }
  ]
}
```

