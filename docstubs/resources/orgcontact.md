---
title: "orgContact resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# orgContact resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List orgContacts](../api/orgcontact-list.md)|[orgContact](../resources/orgcontact.md) collection|List properties and relationships of the [orgContact](../resources/orgcontact.md) objects.|
|[Get orgContact](../api/orgcontact-get.md)|[orgContact](../resources/orgcontact.md)|Read properties and relationships of the [orgContact](../resources/orgcontact.md) object.|
|[Create orgContact](../api/orgcontact-post-contacts.md)|[orgContact](../resources/orgcontact.md)|Create a new [orgContact](../resources/orgcontact.md) object.|
|[Delete orgContact](../api/orgcontact-delete.md)|None|Deletes a [orgContact](../resources/orgcontact.md).|
|[Update orgContact](../api/orgcontact-update.md)|[orgContact](../resources/orgcontact.md)|Update the properties of a [orgContact](../resources/orgcontact.md) object.|
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/orgcontact-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String collection||
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection||
|[restore](../api/orgcontact-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[List directReports](../api/orgcontact-list-directreports.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the directReports navigation property.|
|[Create directReports](../api/orgcontact-post-directreports.md)|[directoryObject](../resources/directoryobject.md)|Create directReports by posting to the directReports collection.|
|[List memberOf](../api/orgcontact-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Create memberOf](../api/orgcontact-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Create memberOf by posting to the memberOf collection.|
|[List transitiveMemberOf](../api/orgcontact-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Create transitiveMemberOf](../api/orgcontact-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Create transitiveMemberOf by posting to the transitiveMemberOf collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addresses|[physicalOfficeAddress](../resources/physicalofficeaddress.md) collection||
|companyName|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|department|String||
|displayName|String||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|jobTitle|String||
|mail|String||
|mailNickname|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|onPremisesSyncEnabled|Boolean||
|phones|[phone](../resources/phone.md) collection||
|proxyAddresses|String collection||
|surname|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directReports|[directoryObject](../resources/directoryobject.md) collection||
|manager|[directoryObject](../resources/directoryobject.md)||
|memberOf|[directoryObject](../resources/directoryobject.md) collection||
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.orgContact",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.orgContact",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalOfficeAddress",
      "city": "String",
      "countryOrRegion": "String",
      "officeLocation": "String",
      "postalCode": "String",
      "state": "String",
      "street": "String"
    }
  ],
  "companyName": "String",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "String",
      "category": "String",
      "propertyCausingError": "String",
      "occurredDateTime": "String (timestamp)"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone",
      "type": "String",
      "number": "String",
      "region": "String",
      "language": "String"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
}
```

