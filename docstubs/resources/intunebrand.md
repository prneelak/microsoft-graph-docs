---
title: "intuneBrand resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# intuneBrand resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|contactITEmailAddress|String|Email address of the person/organization responsible for IT support.|
|contactITName|String|Name of the person/organization responsible for IT support.|
|contactITNotes|String|Text comments regarding the person/organization responsible for IT support.|
|contactITPhoneNumber|String|Phone number of the person/organization responsible for IT support.|
|darkBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a dark background behind the logo.|
|displayName|String|Company/organization name that is displayed to end users.|
|lightBackgroundLogo|[mimeContent](../resources/mimecontent.md)|Logo image displayed in Company Portal apps which have a light background behind the logo.|
|onlineSupportSiteName|String|Display name of the company/organization’s IT helpdesk site.|
|onlineSupportSiteUrl|String|URL to the company/organization’s IT helpdesk site.|
|privacyUrl|String|URL to the company/organization’s privacy policy.|
|showDisplayNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.|
|showLogo|Boolean|Boolean that represents whether the administrator-supplied logo images are shown or not shown.|
|showNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.|
|themeColor|[rgbColor](../resources/rgbcolor.md)|Primary theme color used in the Company Portal applications and web portal.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "showNameNextToLogo": true,
  "showDisplayNameNextToLogo": true
}
```

