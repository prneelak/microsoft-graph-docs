---
title: "List columns"
description: "Get the columnDefinitions from the columns navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List columns

Namespace: microsoft.graph

Get the columnDefinitions from the columns navigation property.

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
GET /sites/{sitesId}/columns
GET /me/joinedTeams/{groupId}/sites/{siteId}/columns
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [columnDefinition](../resources/columndefinition.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_columndefinition"
}
-->
``` http
GET https://graph.microsoft.com/localtest/sites/{sitesId}/columns
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.columndefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2250

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.columnDefinition",
      "id": "fcae4f9b-4f9b-fcae-9b4f-aefc9b4faefc",
      "boolean": {
        "@odata.type": "microsoft.graph.booleanColumn"
      },
      "calculated": {
        "@odata.type": "microsoft.graph.calculatedColumn",
        "format": "Format value",
        "formula": "Formula value",
        "outputType": "Output Type value"
      },
      "choice": {
        "@odata.type": "microsoft.graph.choiceColumn",
        "allowTextEntry": true,
        "choices": [
          "Choices value"
        ],
        "displayAs": "Display As value"
      },
      "columnGroup": "Column Group value",
      "currency": {
        "@odata.type": "microsoft.graph.currencyColumn",
        "locale": "Locale value"
      },
      "dateTime": {
        "@odata.type": "microsoft.graph.dateTimeColumn"
      },
      "defaultValue": {
        "@odata.type": "microsoft.graph.defaultColumnValue",
        "value": "Value value"
      },
      "description": "Description value",
      "displayName": "Display Name value",
      "enforceUniqueValues": true,
      "hidden": true,
      "indexed": true,
      "lookup": {
        "@odata.type": "microsoft.graph.lookupColumn",
        "allowMultipleValues": true,
        "allowUnlimitedLength": true,
        "columnName": "Column Name value",
        "listId": "List Id value",
        "primaryLookupColumnId": "Primary Lookup Column Id value"
      },
      "name": "Name value",
      "number": {
        "@odata.type": "microsoft.graph.numberColumn",
        "decimalPlaces": "Decimal Places value",
        "maximum": "Double",
        "minimum": "Double"
      },
      "personOrGroup": {
        "@odata.type": "microsoft.graph.personOrGroupColumn",
        "allowMultipleSelection": true,
        "chooseFromType": "Choose From Type value"
      },
      "readOnly": true,
      "required": true,
      "text": {
        "@odata.type": "microsoft.graph.textColumn",
        "allowMultipleLines": true,
        "appendChangesToExistingText": true,
        "linesForEditing": 15,
        "maxLength": 9,
        "textType": "Text Type value"
      }
    }
  ]
}
```

