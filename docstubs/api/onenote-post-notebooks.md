---
title: "Add notebooks"
description: "Add notebooks by posting to the notebooks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add notebooks

Namespace: microsoft.graph

Add notebooks by posting to the notebooks collection.

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
POST /me/onenote/notebooks/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [notebook](../resources/notebook.md) object.

The following table shows the properties that are required when you create the [notebook](../resources/notebook.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|isDefault|Boolean||
|userRole|Enumeration|. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|
|isShared|Boolean||
|sectionsUrl|String||
|sectionGroupsUrl|String||
|links|[notebookLinks](../resources/notebooklinks.md)||



## Response
If successful, this method returns a `201 Created` response code and a [notebook](../resources/notebook.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/onenote/notebooks
Content-type: application/json
Content-length: 899

{
  "@odata.type": "#microsoft.graph.notebook",
  "self": "Self value",
  "displayName": "Display Name value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "isDefault": true,
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "https://example.com/sectionsUrl/",
  "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.notebook",
  "id": "81e3ee7b-ee7b-81e3-7bee-e3817beee381",
  "self": "Self value",
  "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
  "displayName": "Display Name value",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2017-01-01T00:01:04.6774489+03:00",
  "isDefault": true,
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "https://example.com/sectionsUrl/",
  "sectionGroupsUrl": "https://example.com/sectionGroupsUrl/",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks",
    "oneNoteClientUrl": {
      "@odata.type": "microsoft.graph.externalLink",
      "href": "Href value"
    },
    "oneNoteWebUrl": {
      "@odata.type": "microsoft.graph.externalLink"
    }
  }
}
```

