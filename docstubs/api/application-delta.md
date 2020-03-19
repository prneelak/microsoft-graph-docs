---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /applications/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [application](../resources/application.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "application_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.application)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "e2f602bd-02bd-e2f6-bd02-f6e2bd02f6e2",
      "deletedDateTime": "2017-01-01T00:00:51.5607674+03:00",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn"
        }
      ],
      "api": {
        "@odata.type": "microsoft.graph.apiApplication"
      },
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "isFallbackPublicClient": true,
      "identifierUris": [
        "Identifier Uris value"
      ],
      "createdDateTime": "2017-01-01T00:00:57.6286041+03:00",
      "publicClient": {
        "@odata.type": "microsoft.graph.publicClientApplication"
      },
      "displayName": "Display Name value",
      "groupMembershipClaims": "Group Membership Claims value",
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl"
      },
      "isDeviceOnlyAuthSupported": true,
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential"
        }
      ],
      "logo": "Stream",
      "oauth2RequirePostResponse": true,
      "optionalClaims": {
        "@odata.type": "microsoft.graph.optionalClaims"
      },
      "parentalControlSettings": {
        "@odata.type": "microsoft.graph.parentalControlSettings"
      },
      "passwordCredentials": [
        {
          "@odata.type": "microsoft.graph.passwordCredential"
        }
      ],
      "publisherDomain": "Publisher Domain value",
      "requiredResourceAccess": [
        {
          "@odata.type": "microsoft.graph.requiredResourceAccess"
        }
      ],
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "ac963d11-3d11-ac96-113d-96ac113d96ac",
      "web": {
        "@odata.type": "microsoft.graph.webApplication"
      }
    }
  ]
}
```

