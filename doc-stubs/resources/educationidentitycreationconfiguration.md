---
title: "educationIdentityCreationConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationIdentityCreationConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [educationIdentitySynchronizationConfiguration](../resources/educationidentitysynchronizationconfiguration.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userDomains|[educationIdentityDomain](../resources/educationidentitydomain.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```

