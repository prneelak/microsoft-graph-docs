---
title: "Get application"
description: "Read properties and relationships of the application object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get application

Namespace: microsoft.graph

Read properties and relationships of the [application](../resources/application.md) object.

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
GET /applications/{applicationsId}
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
If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_application"
}
-->
``` http
GET https://graph.microsoft.com/localtest/applications/{applicationsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5216

{
  "value": {
    "@odata.type": "#microsoft.graph.application",
    "id": "aa825a5b-5a5b-aa82-5b5a-82aa5b5a82aa",
    "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn",
        "id": "585f9ca6-9ca6-585f-a69c-5f58a69c5f58",
        "type": "Type value",
        "properties": [
          {
            "@odata.type": "microsoft.graph.keyValue",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      }
    ],
    "api": {
      "@odata.type": "microsoft.graph.apiApplication",
      "acceptMappedClaims": true,
      "knownClientApplications": [
        "9e5826c2-26c2-9e58-c226-589ec226589e"
      ],
      "preAuthorizedApplications": [
        {
          "@odata.type": "microsoft.graph.preAuthorizedApplication",
          "appId": "App Id value",
          "delegatedPermissionIds": [
            "Delegated Permission Ids value"
          ]
        }
      ],
      "requestedAccessTokenVersion": 11,
      "oauth2PermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope",
          "adminConsentDescription": "Admin Consent Description value",
          "adminConsentDisplayName": "Admin Consent Display Name value",
          "isEnabled": true,
          "origin": "Origin value",
          "userConsentDescription": "User Consent Description value",
          "userConsentDisplayName": "User Consent Display Name value"
        }
      ]
    },
    "appId": "App Id value",
    "applicationTemplateId": "Application Template Id value",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole",
        "allowedMemberTypes": [
          "Allowed Member Types value"
        ],
        "description": "Description value",
        "displayName": "Display Name value"
      }
    ],
    "isFallbackPublicClient": true,
    "identifierUris": [
      "Identifier Uris value"
    ],
    "createdDateTime": "2016-12-31T23:58:32.2073844+03:00",
    "publicClient": {
      "@odata.type": "microsoft.graph.publicClientApplication",
      "redirectUris": [
        "Redirect Uris value"
      ]
    },
    "displayName": "Display Name value",
    "groupMembershipClaims": "Group Membership Claims value",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl",
      "logoUrl": "https://example.com/logoUrl/",
      "marketingUrl": "https://example.com/marketingUrl/",
      "privacyStatementUrl": "https://example.com/privacyStatementUrl/",
      "supportUrl": "https://example.com/supportUrl/",
      "termsOfServiceUrl": "https://example.com/termsOfServiceUrl/"
    },
    "isDeviceOnlyAuthSupported": true,
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential",
        "customKeyIdentifier": "Y3VzdG9tS2V5SWRlbnRpZmllcg==",
        "endDateTime": "2017-01-01T00:02:20.5434752+03:00",
        "keyId": "2d0ca5ff-a5ff-2d0c-ffa5-0c2dffa50c2d",
        "startDateTime": "2017-01-01T00:02:40.1232988+03:00",
        "usage": "Usage value",
        "key": "a2V5"
      }
    ],
    "logo": "Stream",
    "oauth2RequirePostResponse": true,
    "optionalClaims": {
      "@odata.type": "microsoft.graph.optionalClaims",
      "idToken": [
        {
          "@odata.type": "microsoft.graph.optionalClaim",
          "name": "Name value",
          "source": "Source value",
          "essential": true,
          "additionalProperties": [
            "Additional Properties value"
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
    },
    "parentalControlSettings": {
      "@odata.type": "microsoft.graph.parentalControlSettings",
      "countriesBlockedForMinors": [
        "Countries Blocked For Minors value"
      ],
      "legalAgeGroupRule": "Legal Age Group Rule value"
    },
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential",
        "secretText": "Secret Text value",
        "hint": "Hint value"
      }
    ],
    "publisherDomain": "Publisher Domain value",
    "requiredResourceAccess": [
      {
        "@odata.type": "microsoft.graph.requiredResourceAccess",
        "resourceAppId": "Resource App Id value",
        "resourceAccess": [
          {
            "@odata.type": "microsoft.graph.resourceAccess"
          }
        ]
      }
    ],
    "signInAudience": "Sign In Audience value",
    "tags": [
      "Tags value"
    ],
    "tokenEncryptionKeyId": "ae44ea57-ea57-ae44-57ea-44ae57ea44ae",
    "web": {
      "@odata.type": "microsoft.graph.webApplication",
      "homePageUrl": "https://example.com/homePageUrl/",
      "logoutUrl": "https://example.com/logoutUrl/",
      "implicitGrantSettings": {
        "@odata.type": "microsoft.graph.implicitGrantSettings",
        "enableIdTokenIssuance": true,
        "enableAccessTokenIssuance": true
      }
    }
  }
}
```

