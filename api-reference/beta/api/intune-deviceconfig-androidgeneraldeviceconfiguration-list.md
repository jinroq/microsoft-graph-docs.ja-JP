---
title: androidGeneralDeviceConfigurations のリスト
description: androidGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c5a911d6366ad3b3367db2f12250a7db5e5192a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32476021"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="3ce67-103">androidGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="3ce67-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="3ce67-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ce67-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ce67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ce67-106">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3ce67-106">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ce67-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3ce67-107">Prerequisites</span></span>
<span data-ttu-id="3ce67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ce67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce67-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ce67-110">Permission type</span></span>|<span data-ttu-id="3ce67-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ce67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ce67-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ce67-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ce67-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ce67-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ce67-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce67-115">Not supported.</span></span>|
|<span data-ttu-id="3ce67-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ce67-116">Application</span></span>|<span data-ttu-id="3ce67-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ce67-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ce67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3ce67-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce67-119">Request headers</span></span>
|<span data-ttu-id="3ce67-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce67-120">Header</span></span>|<span data-ttu-id="3ce67-121">値</span><span class="sxs-lookup"><span data-stu-id="3ce67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ce67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce67-122">Authorization</span></span>|<span data-ttu-id="3ce67-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ce67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ce67-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3ce67-124">Accept</span></span>|<span data-ttu-id="3ce67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ce67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ce67-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ce67-126">Request body</span></span>
<span data-ttu-id="3ce67-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3ce67-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ce67-128">応答</span><span class="sxs-lookup"><span data-stu-id="3ce67-128">Response</span></span>
<span data-ttu-id="3ce67-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3ce67-129">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce67-130">例</span><span class="sxs-lookup"><span data-stu-id="3ce67-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ce67-131">要求</span><span class="sxs-lookup"><span data-stu-id="3ce67-131">Request</span></span>
<span data-ttu-id="3ce67-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ce67-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3ce67-133">応答</span><span class="sxs-lookup"><span data-stu-id="3ce67-133">Response</span></span>
<span data-ttu-id="3ce67-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ce67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3766

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "appsBlockClipboardSharing": true,
      "appsBlockCopyPaste": true,
      "appsBlockYouTube": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockMessaging": true,
      "cellularBlockVoiceRoaming": true,
      "cellularBlockWiFiTethering": true,
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
      "diagnosticDataBlockSubmission": true,
      "locationServicesBlocked": true,
      "googleAccountBlockAutoSync": true,
      "googlePlayStoreBlocked": true,
      "kioskModeBlockSleepButton": true,
      "kioskModeBlockVolumeButtons": true,
      "dateAndTimeBlockChanges": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "nfcBlocked": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphabetic",
      "passwordRequired": true,
      "powerOffBlocked": true,
      "factoryResetBlocked": true,
      "screenCaptureBlocked": true,
      "deviceSharingAllowed": true,
      "storageBlockGoogleBackup": true,
      "storageBlockRemovableStorage": true,
      "storageRequireDeviceEncryption": true,
      "storageRequireRemovableStorageEncryption": true,
      "voiceAssistantBlocked": true,
      "voiceDialingBlocked": true,
      "webBrowserBlockPopups": true,
      "webBrowserBlockAutofill": true,
      "webBrowserBlockJavaScript": true,
      "webBrowserBlocked": true,
      "webBrowserCookieSettings": "blockAlways",
      "wiFiBlocked": true,
      "appsInstallAllowList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsLaunchBlockList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsHideList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "securityRequireVerifyApps": true
    }
  ]
}
```





