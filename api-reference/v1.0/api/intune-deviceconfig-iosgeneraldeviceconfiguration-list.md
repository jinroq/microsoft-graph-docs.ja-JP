---
title: iosGeneralDeviceConfigurations のリスト
description: iosGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69be37a5dd2d5ec7e3283668d46aa53a23d89a7c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997660"
---
# <a name="list-iosgeneraldeviceconfigurations"></a><span data-ttu-id="2bd7a-103">iosGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="2bd7a-103">List iosGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="2bd7a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bd7a-105">[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-105">List properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bd7a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2bd7a-106">Prerequisites</span></span>
<span data-ttu-id="2bd7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bd7a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bd7a-109">Permission type</span></span>|<span data-ttu-id="2bd7a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bd7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bd7a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bd7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2bd7a-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bd7a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2bd7a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bd7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bd7a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-114">Not supported.</span></span>|
|<span data-ttu-id="2bd7a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bd7a-115">Application</span></span>|<span data-ttu-id="2bd7a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bd7a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bd7a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2bd7a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bd7a-118">Request headers</span></span>
|<span data-ttu-id="2bd7a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bd7a-119">Header</span></span>|<span data-ttu-id="2bd7a-120">値</span><span class="sxs-lookup"><span data-stu-id="2bd7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bd7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bd7a-121">Authorization</span></span>|<span data-ttu-id="2bd7a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bd7a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2bd7a-123">Accept</span></span>|<span data-ttu-id="2bd7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2bd7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bd7a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bd7a-125">Request body</span></span>
<span data-ttu-id="2bd7a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bd7a-127">応答</span><span class="sxs-lookup"><span data-stu-id="2bd7a-127">Response</span></span>
<span data-ttu-id="2bd7a-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-128">If successful, this method returns a `200 OK` response code and a collection of [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bd7a-129">例</span><span class="sxs-lookup"><span data-stu-id="2bd7a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bd7a-130">要求</span><span class="sxs-lookup"><span data-stu-id="2bd7a-130">Request</span></span>
<span data-ttu-id="2bd7a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2bd7a-132">応答</span><span class="sxs-lookup"><span data-stu-id="2bd7a-132">Response</span></span>
<span data-ttu-id="2bd7a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bd7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8922

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
      "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
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
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsVisibilityList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsVisibilityListType": "appsInListCompliant",
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
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
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
        "Email In Domain Suffixes value"
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
      "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
      "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
      "kioskModeRequireAssistiveTouch": true,
      "kioskModeRequireColorInversion": true,
      "kioskModeRequireMonoAudio": true,
      "kioskModeRequireVoiceOver": true,
      "kioskModeRequireZoom": true,
      "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
      "lockScreenBlockControlCenter": true,
      "lockScreenBlockNotificationView": true,
      "lockScreenBlockPassbook": true,
      "lockScreenBlockTodayView": true,
      "mediaContentRatingAustralia": {
        "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingCanada": {
        "@odata.type": "microsoft.graph.mediaContentRatingCanada",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingFrance": {
        "@odata.type": "microsoft.graph.mediaContentRatingFrance",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingGermany": {
        "@odata.type": "microsoft.graph.mediaContentRatingGermany",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingIreland": {
        "@odata.type": "microsoft.graph.mediaContentRatingIreland",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingJapan": {
        "@odata.type": "microsoft.graph.mediaContentRatingJapan",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingNewZealand": {
        "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingUnitedKingdom": {
        "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "mediaContentRatingUnitedStates": {
        "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
        "movieRating": "allBlocked",
        "tvRating": "allBlocked"
      },
      "networkUsageRules": [
        {
          "@odata.type": "microsoft.graph.iosNetworkUsageRule",
          "managedApps": [
            {
              "@odata.type": "microsoft.graph.appListItem",
              "name": "Name value",
              "publisher": "Publisher value",
              "appStoreUrl": "https://example.com/appStoreUrl/",
              "appId": "App Id value"
            }
          ],
          "cellularDataBlockWhenRoaming": true,
          "cellularDataBlocked": true
        }
      ],
      "mediaContentRatingApps": "allBlocked",
      "messagesBlocked": true,
      "notificationsBlockSettingsModification": true,
      "passcodeBlockFingerprintUnlock": true,
      "passcodeBlockFingerprintModification": true,
      "passcodeBlockModification": true,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeSignInFailureCountBeforeWipe": 4,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "podcastsBlocked": true,
      "safariBlockAutofill": true,
      "safariBlockJavaScript": true,
      "safariBlockPopups": true,
      "safariBlocked": true,
      "safariCookieSettings": "blockAlways",
      "safariManagedDomains": [
        "Safari Managed Domains value"
      ],
      "safariPasswordAutoFillDomains": [
        "Safari Password Auto Fill Domains value"
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
  ]
}
```



