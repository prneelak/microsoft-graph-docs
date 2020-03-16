---
title: "applePushNotificationCertificate resource type"
description: "Apple push notification certificate."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# applePushNotificationCertificate resource type


Namespace: microsoft.graph

Apple push notification certificate.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get applePushNotificationCertificate](../api/applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Read properties and relationships of the [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[Update applePushNotificationCertificate](../api/applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/applepushnotificationcertificate.md)|Update the properties of a [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) object.|
|[downloadApplePushNotificationCertificateSigningRequest](../api/applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleIdentifier|String|Apple Id of the account used to create the MDM push certificate.|
|certificate|String||
|expirationDateTime|DateTimeOffset|The expiration date and time for Apple push notification certificate.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified date and time for Apple push notification certificate.|
|topicIdentifier|String|Topic Id.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```

