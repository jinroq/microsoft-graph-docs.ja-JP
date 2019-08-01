---
title: androidGeneralDeviceConfigurations のリスト
description: androidGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d84e44025538206b552c28a1a4c5f081d127ebf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019619"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="a7fd4-103">androidGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="a7fd4-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="a7fd4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7fd4-105">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-105">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7fd4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a7fd4-106">Prerequisites</span></span>
<span data-ttu-id="a7fd4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7fd4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7fd4-109">Permission type</span></span>|<span data-ttu-id="a7fd4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7fd4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7fd4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7fd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7fd4-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7fd4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7fd4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7fd4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7fd4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-114">Not supported.</span></span>|
|<span data-ttu-id="a7fd4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7fd4-115">Application</span></span>|<span data-ttu-id="a7fd4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7fd4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7fd4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7fd4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7fd4-118">Request headers</span></span>
|<span data-ttu-id="a7fd4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7fd4-119">Header</span></span>|<span data-ttu-id="a7fd4-120">値</span><span class="sxs-lookup"><span data-stu-id="a7fd4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7fd4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7fd4-121">Authorization</span></span>|<span data-ttu-id="a7fd4-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7fd4-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a7fd4-123">Accept</span></span>|<span data-ttu-id="a7fd4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7fd4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7fd4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7fd4-125">Request body</span></span>
<span data-ttu-id="a7fd4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7fd4-127">応答</span><span class="sxs-lookup"><span data-stu-id="a7fd4-127">Response</span></span>
<span data-ttu-id="a7fd4-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-128">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7fd4-129">例</span><span class="sxs-lookup"><span data-stu-id="a7fd4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7fd4-130">要求</span><span class="sxs-lookup"><span data-stu-id="a7fd4-130">Request</span></span>
<span data-ttu-id="a7fd4-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a7fd4-132">応答</span><span class="sxs-lookup"><span data-stu-id="a7fd4-132">Response</span></span>
<span data-ttu-id="a7fd4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7fd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



