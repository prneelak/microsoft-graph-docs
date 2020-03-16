---
title: "managedAppRegistration resource type"
description: "The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedAppRegistration resource type


Namespace: microsoft.graph

The ManagedAppEntity is the base entity type for all other entity types under app management workflow.
The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppRegistration](../api/managedappregistration-get.md)|[managedAppRegistration](../resources/managedappregistration.md)|Read properties and relationships of the [managedAppRegistration](../resources/managedappregistration.md) object.|
|[getUserIdsWithFlaggedAppRegistration](../api/managedappregistration-getuseridswithflaggedappregistration.md)|String collection||
|[List appliedPolicies](../api/managedappregistration-list-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the appliedPolicies navigation property.|
|[Add appliedPolicies](../api/managedappregistration-post-appliedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add appliedPolicies by posting to the appliedPolicies collection.|
|[List intendedPolicies](../api/managedappregistration-list-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get the managedAppPolicies from the intendedPolicies navigation property.|
|[Add intendedPolicies](../api/managedappregistration-post-intendedpolicies.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Add intendedPolicies by posting to the intendedPolicies collection.|
|[List operations](../api/managedappregistration-list-operations.md)|[managedAppOperation](../resources/managedappoperation.md) collection|Get the managedAppOperations from the operations navigation property.|
|[Add operations](../api/managedappregistration-post-operations.md)|[managedAppOperation](../resources/managedappoperation.md)|Add operations by posting to the operations collection.|
|[List managedAppRegistrations](../api/user-list-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md) collection|Get the managedAppRegistrations from the managedAppRegistrations navigation property.|
|[Create managedAppRegistrations](../api/user-post-managedappregistrations.md)|[managedAppRegistration](../resources/managedappregistration.md)|Create managedAppRegistrations by posting to the managedAppRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier|
|applicationVersion|String|App version|
|createdDateTime|DateTimeOffset|Date and time of creation|
|deviceName|String|Host device name|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions.|
|deviceType|String|Host device type|
|flaggedReasons|Enumeration collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service.|
|managementSdkVersion|String|App management SDK version|
|platformVersion|String|Operating System version|
|userId|String|The user Id to who this app registration belongs.|
|version|String|Version of the entity.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policys already applied on the registered app when it last synchronized with managment service.|
|intendedPolicies|[managedAppPolicy](../resources/managedapppolicy.md) collection|Zero or more policies admin intended for the app as of now.|
|operations|[managedAppOperation](../resources/managedappoperation.md) collection|Zero or more long running operations triggered on the app registration.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "String"
}
```

