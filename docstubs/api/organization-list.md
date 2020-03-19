---
title: "List organizations"
description: "List properties and relationships of the organization objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List organizations

Namespace: microsoft.graph

List properties and relationships of the [organization](../resources/organization.md) objects.

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
GET /organization
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
If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/organization.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_organization"
}
-->
``` http
GET https://graph.microsoft.com/localtest/organization
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.organization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9914778e-778e-9914-8e77-14998e771499",
      "deletedDateTime": "2017-01-01T00:00:01.2462858+03:00",
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:59:13.3422885+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "9f9e474f-474f-9f9e-4f47-9e9f4f479e9f"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "country": "Country value",
      "countryLetterCode": "Country Letter Code value",
      "createdDateTime": "2016-12-31T23:57:12.4657794+03:00",
      "creationType": "Creation Type value",
      "displayName": "Display Name value",
      "marketingNotificationEmails": [
        "Marketing Notification Emails value"
      ],
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:51.854868+03:00",
      "onPremisesSyncEnabled": true,
      "postalCode": "Postal Code value",
      "preferredLanguage": "Preferred Language value",
      "privacyProfile": {
        "@odata.type": "microsoft.graph.privacyProfile",
        "contactEmail": "Contact Email value",
        "statementUrl": "https://example.com/statementUrl/"
      },
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan",
          "provisioningStatus": "Provisioning Status value"
        }
      ],
      "securityComplianceNotificationMails": [
        "Security Compliance Notification Mails value"
      ],
      "securityComplianceNotificationPhones": [
        "Security Compliance Notification Phones value"
      ],
      "state": "State value",
      "street": "Street value",
      "technicalNotificationMails": [
        "Technical Notification Mails value"
      ],
      "verifiedDomains": [
        {
          "@odata.type": "microsoft.graph.verifiedDomain",
          "capabilities": "Capabilities value",
          "isDefault": true,
          "isInitial": true,
          "name": "Name value",
          "type": "Type value"
        }
      ],
      "mobileDeviceManagementAuthority": "String"
    }
  ]
}
```

