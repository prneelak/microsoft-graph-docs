---
title: "optionalClaims resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# optionalClaims resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessToken|[optionalClaim](../resources/optionalclaim.md) collection||
|idToken|[optionalClaim](../resources/optionalclaim.md) collection||
|saml2Token|[optionalClaim](../resources/optionalclaim.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.optionalClaims",
  "idToken": [
    {
      "@odata.type": "microsoft.graph.optionalClaim",
      "name": "String",
      "source": "String",
      "essential": true,
      "additionalProperties": [
        "String"
      ]
    }
  ],
  "accessToken": [
    {
      "@odata.type": "microsoft.graph.optionalClaim"
    }
  ],
  "saml2Token": [
    {
      "@odata.type": "microsoft.graph.optionalClaim"
    }
  ]
}
```

