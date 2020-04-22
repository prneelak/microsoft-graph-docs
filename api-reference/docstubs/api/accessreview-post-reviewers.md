---
title: "Create reviewers"
description: "Create a new reviewers object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create reviewers

Namespace: microsoft.graph

Create a new reviewers object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /accessReviews/{accessReviewsId}/reviewers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [accessReviewReviewer](../resources/accessreviewreviewer.md) object.

The following table shows the properties that are required when you create the [accessReviewReviewer](../resources/accessreviewreviewer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessReviewReviewer](../resources/accessreviewreviewer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accessreviewreviewer_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/accessReviews/{accessReviewsId}/reviewers
Content-Type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessreviewreviewer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "aedf2ff6-2ff6-aedf-f62f-dfaef62fdfae",
  "displayName": "Display Name value",
  "userPrincipalName": "User Principal Name value"
}
```

