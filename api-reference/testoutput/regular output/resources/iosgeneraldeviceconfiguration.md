---
title: "iosGeneralDeviceConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the iosGeneralDeviceConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosGeneralDeviceConfiguration resource type


Namespace: microsoft.graph

This topic provides descriptions of the declared methods, properties and relationships exposed by the iosGeneralDeviceConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceconfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosGeneralDeviceConfigurations](../api/iosgeneraldeviceconfiguration-list.md)|[iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md) collection|List properties and relationships of the [iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md) objects.|
|[Get iosGeneralDeviceConfiguration](../api/iosgeneraldeviceconfiguration-get.md)|[iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md)|Read properties and relationships of the [iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md) object.|
|[Create iosGeneralDeviceConfiguration](../api/iosgeneraldeviceconfiguration-create.md)|[iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md)|Create a new [iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md) object.|
|[Delete iosGeneralDeviceConfiguration](../api/iosgeneraldeviceconfiguration-delete.md)|None|Deletes a [iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md).|
|[Update iosGeneralDeviceConfiguration](../api/iosgeneraldeviceconfiguration-update.md)|[iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md)|Update the properties of a [iosGeneralDeviceConfiguration](../resources/iosgeneraldeviceconfiguration.md) object.|
|[assign](../api/iosgeneraldeviceconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection||
|[List assignments](../api/iosgeneraldeviceconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/iosgeneraldeviceconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/iosgeneraldeviceconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosgeneraldeviceconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosgeneraldeviceconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosgeneraldeviceconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/iosgeneraldeviceconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/iosgeneraldeviceconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountBlockModification|Boolean|Indicates whether or not to allow account modification when the device is in supervised mode.|
|activationLockAllowWhenSupervised|Boolean|Indicates whether or not to allow activation lock when the device is in the supervised mode.|
|airDropBlocked|Boolean|Indicates whether or not to allow AirDrop when the device is in supervised mode.|
|airDropForceUnmanagedDropTarget|Boolean|Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).|
|airPlayForcePairingPasswordForOutgoingRequests|Boolean|Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.|
|appleNewsBlocked|Boolean|Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).|
|appleWatchBlockPairing|Boolean|Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).|
|appleWatchForceWristDetection|Boolean|Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).|
|appsSingleAppModeList|[appListItem](../resources/applistitem.md) collection|Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode. Supervised only. iOS 7.0 and later. This collection can contain a maximum of 500 elements.|
|appStoreBlockAutomaticDownloads|Boolean|Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).|
|appStoreBlocked|Boolean|Indicates whether or not to block the user from using the App Store.|
|appStoreBlockInAppPurchases|Boolean|Indicates whether or not to block the user from making in app purchases.|
|appStoreBlockUIAppInstallation|Boolean|Indicates whether or not to block the App Store app, not restricting installation through Host apps. Applies to supervised mode only (iOS 9.0 and later).|
|appStoreRequirePassword|Boolean|Indicates whether or not to require a password when using the app store.|
|appsVisibilityList|[appListItem](../resources/applistitem.md) collection|List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later). This collection can contain a maximum of 10000 elements.|
|appsVisibilityListType|Enumeration|Type of list that is in the AppsVisibilityList. Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|bluetoothBlockModification|Boolean|Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).|
|cameraBlocked|Boolean|Indicates whether or not to block the user from accessing the camera of the device.|
|cellularBlockDataRoaming|Boolean|Indicates whether or not to block data roaming.|
|cellularBlockGlobalBackgroundFetchWhileRoaming|Boolean|Indicates whether or not to block global background fetch while roaming.|
|cellularBlockPerAppDataModification|Boolean|Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.|
|cellularBlockPersonalHotspot|Boolean|Indicates whether or not to block Personal Hotspot.|
|cellularBlockVoiceRoaming|Boolean|Indicates whether or not to block voice roaming.|
|certificatesBlockUntrustedTlsCertificates|Boolean|Indicates whether or not to block untrusted TLS certificates.|
|classroomAppBlockRemoteScreenObservation|Boolean|Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).|
|classroomAppForceUnpromptedScreenObservation|Boolean|Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.|
|compliantAppListType|Enumeration|List that is in the AppComplianceList. Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|compliantAppsList|[appListItem](../resources/applistitem.md) collection|List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType). This collection can contain a maximum of 10000 elements.|
|configurationProfileBlockChanges|Boolean|Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|definitionLookupBlocked|Boolean|Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceBlockEnableRestrictions|Boolean|Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.|
|deviceBlockEraseContentAndSettings|Boolean|Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.|
|deviceBlockNameModification|Boolean|Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).|
|diagnosticDataBlockSubmission|Boolean|Indicates whether or not to block diagnostic data submission.|
|diagnosticDataBlockSubmissionModification|Boolean|Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|documentsBlockManagedDocumentsInUnmanagedApps|Boolean|Indicates whether or not to block the user from viewing managed documents in unmanaged apps.|
|documentsBlockUnmanagedDocumentsInManagedApps|Boolean|Indicates whether or not to block the user from viewing unmanaged documents in managed apps.|
|emailInDomainSuffixes|String collection|An email address lacking a suffix that matches any of these strings will be considered out-of-domain.|
|enterpriseAppBlockTrust|Boolean|Indicates whether or not to block the user from trusting an enterprise app.|
|enterpriseAppBlockTrustModification|Boolean|Indicates whether or not to block the user from modifying the enterprise app trust settings.|
|faceTimeBlocked|Boolean|Indicates whether or not to block the user from using FaceTime.|
|findMyFriendsBlocked|Boolean|Indicates whether or not to block Find My Friends when the device is in supervised mode.|
|gameCenterBlocked|Boolean|Indicates whether or not to block the user from using Game Center when the device is in supervised mode.|
|gamingBlockGameCenterFriends|Boolean|Indicates whether or not to block the user from having friends in Game Center.|
|gamingBlockMultiplayer|Boolean|Indicates whether or not to block the user from using multiplayer gaming.|
|hostPairingBlocked|Boolean|indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.|
|iBooksStoreBlocked|Boolean|Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.|
|iBooksStoreBlockErotica|Boolean|Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.|
|iCloudBlockActivityContinuation|Boolean|Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.|
|iCloudBlockBackup|Boolean|Indicates whether or not to block iCloud backup.|
|iCloudBlockDocumentSync|Boolean|Indicates whether or not to block iCloud document sync.|
|iCloudBlockManagedAppsSync|Boolean|Indicates whether or not to block Managed Apps Cloud Sync.|
|iCloudBlockPhotoLibrary|Boolean|Indicates whether or not to block iCloud Photo Library.|
|iCloudBlockPhotoStreamSync|Boolean|Indicates whether or not to block iCloud Photo Stream Sync.|
|iCloudBlockSharedPhotoStream|Boolean|Indicates whether or not to block Shared Photo Stream.|
|iCloudRequireEncryptedBackup|Boolean|Indicates whether or not to require backups to iCloud be encrypted.|
|id|String| Inherited from [entity](../resources/entity.md)|
|iTunesBlockExplicitContent|Boolean|Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.|
|iTunesBlockMusicService|Boolean|Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).|
|iTunesBlockRadio|Boolean|Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).|
|keyboardBlockAutoCorrect|Boolean|Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).|
|keyboardBlockDictation|Boolean|Indicates whether or not to block the user from using dictation input when the device is in supervised mode.|
|keyboardBlockPredictive|Boolean|Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).|
|keyboardBlockShortcuts|Boolean|Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).|
|keyboardBlockSpellCheck|Boolean|Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).|
|kioskModeAllowAssistiveSpeak|Boolean|Indicates whether or not to allow assistive speak while in kiosk mode.|
|kioskModeAllowAssistiveTouchSettings|Boolean|Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.|
|kioskModeAllowAutoLock|Boolean|Indicates whether or not to allow device auto lock while in kiosk mode.|
|kioskModeAllowColorInversionSettings|Boolean|Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.|
|kioskModeAllowRingerSwitch|Boolean|Indicates whether or not to allow use of the ringer switch while in kiosk mode.|
|kioskModeAllowScreenRotation|Boolean|Indicates whether or not to allow screen rotation while in kiosk mode.|
|kioskModeAllowSleepButton|Boolean|Indicates whether or not to allow use of the sleep button while in kiosk mode.|
|kioskModeAllowTouchscreen|Boolean|Indicates whether or not to allow use of the touchscreen while in kiosk mode.|
|kioskModeAllowVoiceOverSettings|Boolean|Indicates whether or not to allow access to the voice over settings while in kiosk mode.|
|kioskModeAllowVolumeButtons|Boolean|Indicates whether or not to allow use of the volume buttons while in kiosk mode.|
|kioskModeAllowZoomSettings|Boolean|Indicates whether or not to allow access to the zoom settings while in kiosk mode.|
|kioskModeAppStoreUrl|String|URL in the app store to the app to use for kiosk mode. Use if KioskModeManagedAppId is not known.|
|kioskModeBuiltInAppId|String|ID for built-in apps to use for kiosk mode. Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.|
|kioskModeManagedAppId|String|Managed app id of the app to use for kiosk mode. If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.|
|kioskModeRequireAssistiveTouch|Boolean|Indicates whether or not to require assistive touch while in kiosk mode.|
|kioskModeRequireColorInversion|Boolean|Indicates whether or not to require color inversion while in kiosk mode.|
|kioskModeRequireMonoAudio|Boolean|Indicates whether or not to require mono audio while in kiosk mode.|
|kioskModeRequireVoiceOver|Boolean|Indicates whether or not to require voice over while in kiosk mode.|
|kioskModeRequireZoom|Boolean|Indicates whether or not to require zoom while in kiosk mode.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|lockScreenBlockControlCenter|Boolean|Indicates whether or not to block the user from using control center on the lock screen.|
|lockScreenBlockNotificationView|Boolean|Indicates whether or not to block the user from using the notification view on the lock screen.|
|lockScreenBlockPassbook|Boolean|Indicates whether or not to block the user from using passbook when the device is locked.|
|lockScreenBlockTodayView|Boolean|Indicates whether or not to block the user from using the Today View on the lock screen.|
|mediaContentRatingApps|Enumeration|Media content rating settings for Apps. Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.|
|mediaContentRatingAustralia|[mediaContentRatingAustralia](../resources/mediacontentratingaustralia.md)|Media content rating settings for Australia|
|mediaContentRatingCanada|[mediaContentRatingCanada](../resources/mediacontentratingcanada.md)|Media content rating settings for Canada|
|mediaContentRatingFrance|[mediaContentRatingFrance](../resources/mediacontentratingfrance.md)|Media content rating settings for France|
|mediaContentRatingGermany|[mediaContentRatingGermany](../resources/mediacontentratinggermany.md)|Media content rating settings for Germany|
|mediaContentRatingIreland|[mediaContentRatingIreland](../resources/mediacontentratingireland.md)|Media content rating settings for Ireland|
|mediaContentRatingJapan|[mediaContentRatingJapan](../resources/mediacontentratingjapan.md)|Media content rating settings for Japan|
|mediaContentRatingNewZealand|[mediaContentRatingNewZealand](../resources/mediacontentratingnewzealand.md)|Media content rating settings for New Zealand|
|mediaContentRatingUnitedKingdom|[mediaContentRatingUnitedKingdom](../resources/mediacontentratingunitedkingdom.md)|Media content rating settings for United Kingdom|
|mediaContentRatingUnitedStates|[mediaContentRatingUnitedStates](../resources/mediacontentratingunitedstates.md)|Media content rating settings for United States|
|messagesBlocked|Boolean|Indicates whether or not to block the user from using the Messages app on the supervised device.|
|networkUsageRules|[iosNetworkUsageRule](../resources/iosnetworkusagerule.md) collection|List of managed apps and the network rules that applies to them. This collection can contain a maximum of 1000 elements.|
|notificationsBlockSettingsModification|Boolean|Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).|
|passcodeBlockFingerprintModification|Boolean|Block modification of registered Touch ID fingerprints when in supervised mode.|
|passcodeBlockFingerprintUnlock|Boolean|Indicates whether or not to block fingerprint unlock.|
|passcodeBlockModification|Boolean|Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).|
|passcodeBlockSimple|Boolean|Indicates whether or not to block simple passcodes.|
|passcodeExpirationDays|Int32|Number of days before the passcode expires. Valid values 1 to 65535|
|passcodeMinimumCharacterSetCount|Int32|Number of character sets a passcode must contain. Valid values 0 to 4|
|passcodeMinimumLength|Int32|Minimum length of passcode. Valid values 4 to 14|
|passcodeMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity before a passcode is required.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Minutes of inactivity before the screen times out.|
|passcodePreviousPasscodeBlockCount|Int32|Number of previous passcodes to block. Valid values 1 to 24|
|passcodeRequired|Boolean|Indicates whether or not to require a passcode.|
|passcodeRequiredType|Enumeration|Type of passcode that is required. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeSignInFailureCountBeforeWipe|Int32|Number of sign in failures allowed before wiping the device. Valid values 4 to 11|
|podcastsBlocked|Boolean|Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).|
|safariBlockAutofill|Boolean|Indicates whether or not to block the user from using Auto fill in Safari.|
|safariBlocked|Boolean|Indicates whether or not to block the user from using Safari.|
|safariBlockJavaScript|Boolean|Indicates whether or not to block JavaScript in Safari.|
|safariBlockPopups|Boolean|Indicates whether or not to block popups in Safari.|
|safariCookieSettings|Enumeration|Cookie settings for Safari. Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|safariManagedDomains|String collection|URLs matching the patterns listed here will be considered managed.|
|safariPasswordAutoFillDomains|String collection|Users can save passwords in Safari only from URLs matching the patterns listed here. Applies to devices in supervised mode (iOS 9.3 and later).|
|safariRequireFraudWarning|Boolean|Indicates whether or not to require fraud warning in Safari.|
|screenCaptureBlocked|Boolean|Indicates whether or not to block the user from taking Screenshots.|
|siriBlocked|Boolean|Indicates whether or not to block the user from using Siri.|
|siriBlockedWhenLocked|Boolean|Indicates whether or not to block the user from using Siri when locked.|
|siriBlockUserGeneratedContent|Boolean|Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.|
|siriRequireProfanityFilter|Boolean|Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.|
|spotlightBlockInternetResults|Boolean|Indicates whether or not to block Spotlight search from returning internet results on supervised device.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|voiceDialingBlocked|Boolean|Indicates whether or not to block voice dialing.|
|wallpaperBlockModification|Boolean|Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .|
|wiFiConnectOnlyToConfiguredNetworks|Boolean|Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceconfigurationuserstatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosGeneralDeviceConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "appsVisibilityListType": "String",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem"
    }
  ],
  "compliantAppListType": "String",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "String"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "String",
  "kioskModeBuiltInAppId": "String",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "String",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "String",
    "tvRating": "String"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "String",
    "tvRating": "String"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "String",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 1024,
  "passcodeMinimumLength": 1024,
  "passcodeMinutesOfInactivityBeforeLock": 1024,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passcodeMinimumCharacterSetCount": 1024,
  "passcodePreviousPasscodeBlockCount": 1024,
  "passcodeSignInFailureCountBeforeWipe": 1024,
  "passcodeRequiredType": "String",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "String",
  "safariManagedDomains": [
    "String"
  ],
  "safariPasswordAutoFillDomains": [
    "String"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

