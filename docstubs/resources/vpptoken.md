---
title: "vppToken resource type"
description: "You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education. This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune. You can then synchronize your volume purchase information with Intune and track your volume-purchased app use. You can upload multiple Apple VPP Business or Education tokens."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# vppToken resource type


Namespace: microsoft.graph

You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education. This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune. You can then synchronize your volume purchase information with Intune and track your volume-purchased app use. You can upload multiple Apple VPP Business or Education tokens.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get vppToken](../api/vpptoken-get.md)|[vppToken](../resources/vpptoken.md)|Read properties and relationships of the [vppToken](../resources/vpptoken.md) object.|
|[Update vppToken](../api/vpptoken-update.md)|[vppToken](../resources/vpptoken.md)|Update the properties of a [vppToken](../resources/vpptoken.md) object.|
|[syncLicenses](../api/vpptoken-synclicenses.md)|[vppToken](../resources/vpptoken.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The apple Id associated with the given Apple Volume Purchase Program Token.|
|automaticallyUpdateApps|Boolean|Whether or not apps for the VPP token will be automatically updated.|
|countryOrRegion|String|Whether or not apps for the VPP token will be automatically updated.|
|expirationDateTime|DateTimeOffset|The expiration date time of the Apple Volume Purchase Program Token.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modification date time associated with the Apple Volume Purchase Program Token.|
|lastSyncDateTime|DateTimeOffset|The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.|
|lastSyncStatus|Enumeration|Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. Possible values are: `none`, `inProgress`, `completed`, `failed`. Possible values are: `none`, `inProgress`, `completed`, `failed`.|
|organizationName|String|The organization associated with the Apple Volume Purchase Program Token|
|state|Enumeration|Current state of the Apple Volume Purchase Program Token. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|token|String|The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.|
|vppTokenAccountType|Enumeration|The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. Possible values are: `business`, `education`. Possible values are: `business`, `education`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```

