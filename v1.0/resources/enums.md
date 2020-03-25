---
title: "Enum values"
description: "Microsoft Graph enumeration values."
localization_priority: Normal
author: ""
ms.prod: ""
doc_type: enumPageType
---

### contactRelationship values

|Member|Value|Description|
|:---|:---|:---|
|parent|0|The user's parent.|
|relative|1| The user's relative.|
|aide|2| The user's aide.|
|doctor|3| The user's doctor.|
|guardian|4| The user's guardian.|
|child|5| The user's child.|
|other|6| An unspecified relationship to the user.|
|unknownFutureValue|7| Marker value for future compatibility.|

### timeZoneStandard values

| Member
|:-----------------
| windows
| iana


### freeBusyStatus values

| Member            |Value
|:------------------|:-------
| free              | 0
| tentative         | 1
| busy              | 2
| oof               | 3
| workingElsewhere  | 4
| unknown           | -1


### attendeeType values

| Member
|:-------------------------
| required
| optional
| resource


### externalAudienceScope values

| Member
|:-------------------------
| none
| contactsOnly
| all


### automaticRepliesStatus values

| Member
|:-------------------------
| disabled
| alwaysEnabled
| scheduled


### calendarColor values

| Member     | Value
|:-----------|:----------
| auto       | -1
| lightBlue  | 0
| lightGreen | 1
| lightOrange| 2
| lightGray  | 3
| lightYellow| 4
| lightTeal  | 5
| lightPink  | 6
| lightBrown | 7
| lightRed   | 8
| maxColor   | 9


### educationExternalSource values

| Member
|:-------------------------
| sis
| manual
| unknownFutureValue


### educationGender values

| Member
|:-------------------------
| female
| male
| other
| unknownFutureValue


### eventType values

| Member
|:-------------------------
| singleInstance
| occurrence
| exception
| seriesMaster


### sensitivity values

| Member
|:-------------------------
| normal
| personal
| private
| confidential


### importance values

| Member
|:-------------------------
| low
| normal
| high


### educationUserRole values
| Member
|:---------------------
| student
| teacher

### meetingMessageType values

| Member
|:-----------------
| none
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTenativelyAccepted
| meetingDeclined


### followupFlagStatus values

| Member
|:-------------------------
| notFlagged
| complete
| flagged


### inferenceClassificationType values

| Member
|:-----------------
| focused
| other


### iosNotificationAlertType values

| Member
|:-------------------------
| deviceDefault
| banner
| modal
| none

### deviceEnrollmentFailureReason values

| Member
|:-------------
| unknown
| authentication
| authorization
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### bodyType values
| Member
|:---------
| text
| html


### locationType values

| Member
|:-------------------------
| default
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| hotel
| restaurant
| localBusiness
| postalAddress

### locationUniqueIdType values

| Member
|:-------------------------
| unknown
| locationStore
| directory
| private
| bing


### messageActionFlag values

| Member
|:-------------------------
| any
| call
| doNotForward
| followUp
| fyi
| forward
| noResponseNecessary
| read
| reply
| replyToAll
| review


### onenoteUserRole values

| Member      | Value
|:------------|:------------
| Owner       | 0
| Contributor | 1
| Reader      | 2
| None        | -1


### operationStatus values

| Member
|:-----------------
| NotStarted
| Running
| Completed
| Failed


### onenotePatchActionType values

| Member
|:-------------------------
| Replace
| Append
| Delete
| Insert
| Prepend

### onenotePatchInsertPosition values

| Member
|:-------------------------
| After
| Before


### phoneType values

| Member
|:-------------------------
| home
| business
| mobile
| other
| assistant
| homeFax
| businessFax
| otherFax
| pager
| radio


### plannerPreviewType values

| Member
|:-------------------------
| automatic
| noPreview
| checklist
| description
| reference


### status values

| Member
|:-----------------
| active
| updated
| deleted
| ignored
| unknownFutureValue


### weekIndex values

| Member
|:-------------------------
| first
| second
| third
| fourth
| last


### dayOfWeek values

| Member
|:-------------------------
| sunday
| monday
| tuesday
| wednesday
| thursday
| friday
| saturday

### recurrencePatternType values

| Member
|:-------------------------
| daily
| weekly
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### recurrenceRangeType values

| Member
|:-------------------------
| endDate
| noEnd
| numbered


### onenoteSourceService values
| Member
|:---------------------
| Unknown
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### responseType values

| Member
|:-------------------------
| none
| organizer
| tentativelyAccepted
| accepted
| declined
| notResponded


### activityDomain values

| Member
|:-------------------------
| unknown
| work
| personal
| unrestricted


### websiteType values

| Member
|:-------------------------
| other
| home
| work
| blog
| profile


### categoryColor values

| Member   |Value
|:---------|:--------
| none     | -1
| preset0  | 0
| preset1  | 1
| preset2  | 2
| preset3  | 3
| preset4  | 4
| preset5  | 5
| preset6  | 6
| preset7  | 7
| preset8  | 8
| preset9  | 9
| preset10 | 10
| preset11 | 11
| preset12 | 12
| preset13 | 13
| preset14 | 14
| preset15 | 15
| preset16 | 16
| preset17 | 17
| preset18 | 18
| preset19 | 19
| preset20 | 20
| preset21 | 21
| preset22 | 22
| preset23 | 23
| preset24 | 24

### alertFeedback values

Possible feedback values on the alert provided by an analyst.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown.|
|truePositive|1|Alert is true-positive.|
|falsePositive|2| Alert is false-positive.|
|benignPositive|3| Alert is benign-positive.|

### fileHashType values

Enum for file hash types.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown type.|
|sha1|1|SHA1 hash type.|
|sha256|2| SHA256 hash type.|
|md5|3| MD5 hash type.|
|authenticodeHash256|4| AuthenticodeHash256 hash type.|
|lsHash|5| LsHash hash type.|
|ctph|6| CTPH hash type.|
|peSha1|7| PESHA1 hash type.|
|peSha256|8| PESHA256 hash type.|

### connectionDirection values

Enum for the direction of the network connection (inbound/outbound).

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown connection.|
|inbound|1|Inbound connection.|
|outbound|2| Outbound connection.|

### connectionStatus values

Enum for the status of connections.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown connection status.|
|attempted|1|Connection attempted.|
|succeeded|2| Connection succeeded.|
|blocked|3| Connection blocked.|
|failed|4| Connection failed.|

### processIntegrityLevel values

Possible integrity level values of the process.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown.|
|untrusted|10|Integrity level is Untrusted.|
|low|20| Integrity level is Low.|
|medium|30| Integrity level is Medium.|
|high|40| Integrity level is High.|
|system|50| Integrity level is System.|

### registryHive values

Enum for registry hives as defined by [/windows/desktop/sysinfo/registry-hives](/windows/desktop/sysinfo/registry-hives).

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown hive.|
|currentConfig|1|HKEY_CURRENT_CONFIG hive.|
|currentUser|2| HKEY_CURRENT_USER hive.|
|localMachineSam|3| HKEY_LOCAL_MACHINE\SAM hive.|
|localMachineSamSoftware|4| HKEY_LOCAL_MACHINE\Software hive.|
|localMachineSystem|5| HKEY_LOCAL_MACHINE\System hive.|
|usersDefault|6| HKEY_USERS\\.DEFAULT hive.|

### registryOperation values

Operation that changed the registry key name and/or value.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown registry value type.|
|create|1|Create registry.|
|modify|2|Modify registry.|
|delete|3|Delete registry.|

### registryValueType values

Enum for registry value types as defined by [/windows/desktop/sysinfo/registry-value-types](/windows/desktop/sysinfo/registry-value-types).

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown registry value type.|
|binary|1|REG_BINARY registry value type.|
|dword|2| REG_DWORD registry value type.|
|dwordLittleEndian|3| REG_DWORD_LITTLE_ENDIAN registry value type.|
|dwordBigEndian|4| REG_DWORD_BIG_ENDIAN registry value type.|
|expandSz|5| REG_EXPAND_SZ registry value type.|
|link|6| REG_LINK registry value type.|
|multiSz|7| REG_MULTI_SZ registry value type.|
|none|8| REG_NONE registry value type.|
|qword|9| REG_QWORD registry value type.|
|qwordlittleEndian|10| REG_QWORD_LITTLE_ENDIAN registry value type.|
|sz|11| REG_SZ registry value type.|

### alertSeverity values

Enum for severity of alerts.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Severity is unknown.|
|informational|1|Severity is only for information.|
|low|2| Severity is low.|
|medium|3| Severity is medium.|
|high|4| Severity is high.|

### alertStatus values

Possible values of an Alert lifecycle status (stage).

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown status.|
|newAlert|10| Alert is new.|
|inProgress|20|Alert is in progress.|
|resolved|30|Alert is resolved.|

### emailRole values
Possible values for email roles.

|Member|Value|Description|
|:---|:---|:---|
|unknown|0|Unknown Role.|
|sender|1|Sender of the email.|
|recipient|2|Recipient of the email.|

### logonType values

Possible values for the method of user signin.

|Member|Value|Description|
|:---|:---|:---|
|unknown|-1|Unknown.|
|interactive|0|Logon is interactive.|
|remoteInteractive|1| Logon is remote interactive.|
|network|2| Logon is network.|
|batch|3| Logon is batch.|
|service|4| Logon is service.|

### userAccountSecurityType values

Possible values for user account types (group membership), per Windows definition.

|Member|Member|Description|
|:---|:---|:---|
|unknown|-1|Unknown.|
|standard|0|Member of Standard Users group.|
|power|1| Member of Power Users group.|
|administrator|2| Member of Administrators group.|

### riskDetail values

| Member
|:-------------------------
| adminGeneratedTemporaryPassword
| userPerformedSecuredPasswordChange
| userPerformedSecuredPasswordReset
| adminConfirmedSigninSafe
| aiConfirmedSigninSafe
| userPassedMFADrivenByRiskBasedPolicy
| adminDismissedAllRiskForUser
| adminConfirmedSigninCompromised
| unknownFutureValue

### riskEventTypes values

| Member
|:-------------------------
| unlikelyTravel
| anonymizedIPAddress
| maliciousIPAddress
| unfamiliarFeatures
| malwareInfectedIPAddress
| suspiciousIPAddress
| leakedCredentials
| investigationsThreatIntelligence
| generic
| unknownFutureValue

### riskLevel values

| Member
|:-------------------------
| none
| low
| medium
| high
| hidden
| unknownFutureValue

### riskState values

| Member
|:-------------------------
| none
| confirmedSafe
| remediated
| dismissed
| atRisk
| confirmedCompromised
| unknownFutureValue

### exchangeIdFormat values

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|
