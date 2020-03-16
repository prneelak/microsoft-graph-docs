---
title: "alert resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# alert resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get alert](../api/alert-get.md)|[alert](../resources/alert.md)|Read properties and relationships of the [alert](../resources/alert.md) object.|
|[Update alert](../api/alert-update.md)|[alert](../resources/alert.md)|Update the properties of a [alert](../resources/alert.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
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
|feedback|Enumeration|. Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`, `unknownFutureValue`.|
|fileStates|[fileSecurityState](../resources/filesecuritystate.md) collection||
|historyStates|[alertHistoryState](../resources/alerthistorystate.md) collection||
|hostStates|[hostSecurityState](../resources/hostsecuritystate.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|malwareStates|[malwareState](../resources/malwarestate.md) collection||
|networkConnections|[networkConnection](../resources/networkconnection.md) collection||
|processes|[process](../resources/process.md) collection||
|recommendedActions|String collection||
|registryKeyStates|[registryKeyState](../resources/registrykeystate.md) collection||
|severity|Enumeration|. Possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`.|
|sourceMaterials|String collection||
|status|Enumeration|. Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`, `unknownFutureValue`.|
|tags|String collection||
|title|String||
|triggers|[alertTrigger](../resources/alerttrigger.md) collection||
|userStates|[userSecurityState](../resources/usersecuritystate.md) collection||
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)||
|vulnerabilityStates|[vulnerabilityState](../resources/vulnerabilitystate.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alert",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.alert",
  "id": "String (identifier)",
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [
    {
      "@odata.type": "microsoft.graph.cloudAppSecurityState"
    }
  ],
  "comments": [
    "String"
  ],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": [
    "String"
  ],
  "eventDateTime": "String (timestamp)",
  "feedback": "String",
  "fileStates": [
    {
      "@odata.type": "microsoft.graph.fileSecurityState"
    }
  ],
  "historyStates": [
    {
      "@odata.type": "microsoft.graph.alertHistoryState"
    }
  ],
  "hostStates": [
    {
      "@odata.type": "microsoft.graph.hostSecurityState"
    }
  ],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [
    {
      "@odata.type": "microsoft.graph.malwareState"
    }
  ],
  "networkConnections": [
    {
      "@odata.type": "microsoft.graph.networkConnection"
    }
  ],
  "processes": [
    {
      "@odata.type": "microsoft.graph.process"
    }
  ],
  "recommendedActions": [
    "String"
  ],
  "registryKeyStates": [
    {
      "@odata.type": "microsoft.graph.registryKeyState"
    }
  ],
  "severity": "String",
  "sourceMaterials": [
    "String"
  ],
  "status": "String",
  "tags": [
    "String"
  ],
  "title": "String",
  "triggers": [
    {
      "@odata.type": "microsoft.graph.alertTrigger"
    }
  ],
  "userStates": [
    {
      "@odata.type": "microsoft.graph.userSecurityState"
    }
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  },
  "vulnerabilityStates": [
    {
      "@odata.type": "microsoft.graph.vulnerabilityState"
    }
  ]
}
```

