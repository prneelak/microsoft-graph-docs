---
title: "Add alerts"
description: "Add alerts by posting to the alerts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add alerts

Namespace: microsoft.graph

Add alerts by posting to the alerts collection.

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
POST /Security/alerts/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [alert](../resources/alert.md) object.

The following table shows the properties that are required when you create the [alert](../resources/alert.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|activityGroupName|String||
|assignedTo|String||
|azureSubscriptionId|String||
|azureTenantId|String||
|category|String||
|closedDateTime|DateTimeOffset||
|cloudAppStates|[cloudAppSecurityState](../resources/cloudappsecuritystate.md) collection||
|comments|String collection||
|confidence|Int32||
|createdDateTime|DateTimeOffset||
|description|String||
|detectionIds|String collection||
|eventDateTime|DateTimeOffset||
|feedback|Enumeration| Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|fileStates|[fileSecurityState](../resources/filesecuritystate.md) collection||
|historyStates|[alertHistoryState](../resources/alerthistorystate.md) collection||
|hostStates|[hostSecurityState](../resources/hostsecuritystate.md) collection||
|lastModifiedDateTime|DateTimeOffset||
|malwareStates|[malwareState](../resources/malwarestate.md) collection||
|networkConnections|[networkConnection](../resources/networkconnection.md) collection||
|processes|[process](../resources/process.md) collection||
|recommendedActions|String collection||
|registryKeyStates|[registryKeyState](../resources/registrykeystate.md) collection||
|severity|Enumeration| Possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.|
|sourceMaterials|String collection||
|status|Enumeration| Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|tags|String collection||
|title|String||
|triggers|[alertTrigger](../resources/alerttrigger.md) collection||
|userStates|[userSecurityState](../resources/usersecuritystate.md) collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [alert](../resources/alert.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_alert_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/alerts
Content-type: application/json
Content-length: 5209

{
  "@odata.type": "#microsoft.graph.alert",
  "activityGroupName": "Activity Group Name value",
  "assignedTo": "Assigned To value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "category": "Category value",
  "closedDateTime": "2016-12-31T23:59:32.6411881+03:00",
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
  "description": "Description value",
  "detectionIds": [
    "Detection Ids value"
  ],
  "eventDateTime": "2016-12-31T23:58:53.8501245+03:00",
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
      "updatedDateTime": "2017-01-01T00:00:30.4198162+03:00",
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
      "domainRegisteredDateTime": "2017-01-01T00:03:12.2448626+03:00",
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
      "parentProcessCreatedDateTime": "2016-12-31T23:58:10.5189949+03:00",
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
      "logonDateTime": "2016-12-31T23:59:48.4074552+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5380

{
  "@odata.type": "#microsoft.graph.alert",
  "id": "1f45f39f-f39f-1f45-9ff3-451f9ff3451f",
  "activityGroupName": "Activity Group Name value",
  "assignedTo": "Assigned To value",
  "azureSubscriptionId": "Azure Subscription Id value",
  "azureTenantId": "Azure Tenant Id value",
  "category": "Category value",
  "closedDateTime": "2016-12-31T23:59:32.6411881+03:00",
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
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "description": "Description value",
  "detectionIds": [
    "Detection Ids value"
  ],
  "eventDateTime": "2016-12-31T23:58:53.8501245+03:00",
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
      "updatedDateTime": "2017-01-01T00:00:30.4198162+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
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
      "domainRegisteredDateTime": "2017-01-01T00:03:12.2448626+03:00",
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
      "parentProcessCreatedDateTime": "2016-12-31T23:58:10.5189949+03:00",
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
      "logonDateTime": "2016-12-31T23:59:48.4074552+03:00",
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
```

