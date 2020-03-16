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
GET /users/delta
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [user](../resources/user.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_delta"
}
-->
``` http
GET https://graph.microsoft.com/localtest/users/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3909

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "45ffba21-ba21-45ff-21ba-ff4521baff45",
      "deletedDateTime": "2016-12-31T23:58:44.8337022+03:00",
      "accountEnabled": true,
      "ageGroup": "Age Group value",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "companyName": "Company Name value",
      "consentProvidedForMinor": "Consent Provided For Minor value",
      "country": "Country value",
      "department": "Department value",
      "displayName": "Display Name value",
      "employeeId": "Employee Id value",
      "faxNumber": "Fax Number value",
      "givenName": "Given Name value",
      "imAddresses": [
        "Im Addresses value"
      ],
      "isResourceAccount": true,
      "jobTitle": "Job Title value",
      "lastPasswordChangeDateTime": "2017-01-01T00:01:16.5787591+03:00",
      "legalAgeGroupClassification": "Legal Age Group Classification value",
      "licenseAssignmentStates": [
        {
          "@odata.type": "microsoft.graph.licenseAssignmentState"
        }
      ],
      "mail": "Mail value",
      "mailNickname": "Mail Nickname value",
      "mobilePhone": "Mobile Phone value",
      "onPremisesDistinguishedName": "On Premises Distinguished Name value",
      "onPremisesExtensionAttributes": {
        "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
      },
      "onPremisesImmutableId": "On Premises Immutable Id value",
      "onPremisesLastSyncDateTime": "2017-01-01T00:03:13.2795175+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError"
        }
      ],
      "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
      "onPremisesSyncEnabled": true,
      "onPremisesDomainName": "On Premises Domain Name value",
      "onPremisesSamAccountName": "On Premises Sam Account Name value",
      "onPremisesUserPrincipalName": "On Premises User Principal Name value",
      "otherMails": [
        "Other Mails value"
      ],
      "passwordPolicies": "Password Policies value",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "Office Location value",
      "postalCode": "Postal Code value",
      "preferredLanguage": "Preferred Language value",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "proxyAddresses": [
        "Proxy Addresses value"
      ],
      "showInAddressList": true,
      "signInSessionsValidFromDateTime": "2016-12-31T23:57:23.5397067+03:00",
      "state": "State value",
      "streetAddress": "Street Address value",
      "surname": "Surname value",
      "usageLocation": "Usage Location value",
      "userPrincipalName": "User Principal Name value",
      "userType": "User Type value",
      "mailboxSettings": {
        "@odata.type": "microsoft.graph.mailboxSettings"
      },
      "deviceEnrollmentLimit": 5,
      "aboutMe": "About Me value",
      "birthday": "2016-12-31T23:59:18.574384+03:00",
      "hireDate": "2016-12-31T23:57:52.2874487+03:00",
      "interests": [
        "Interests value"
      ],
      "mySite": "My Site value",
      "pastProjects": [
        "Past Projects value"
      ],
      "preferredName": "Preferred Name value",
      "responsibilities": [
        "Responsibilities value"
      ],
      "schools": [
        "Schools value"
      ],
      "skills": [
        "Skills value"
      ]
    }
  ]
}
```

