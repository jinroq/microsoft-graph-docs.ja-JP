---
title: Get androidGeneralDeviceConfiguration
description: androidGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2702dc21f9892db759188ddbef3b050302d18e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553541"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="8499a-103">Get androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8499a-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8499a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8499a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8499a-105">[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8499a-105">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8499a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8499a-106">Prerequisites</span></span>
<span data-ttu-id="8499a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8499a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8499a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8499a-109">Permission type</span></span>|<span data-ttu-id="8499a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8499a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8499a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8499a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8499a-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8499a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8499a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8499a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8499a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8499a-114">Not supported.</span></span>|
|<span data-ttu-id="8499a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8499a-115">Application</span></span>|<span data-ttu-id="8499a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8499a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8499a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8499a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8499a-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8499a-118">Optional query parameters</span></span>
<span data-ttu-id="8499a-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8499a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8499a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8499a-120">Request headers</span></span>
|<span data-ttu-id="8499a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8499a-121">Header</span></span>|<span data-ttu-id="8499a-122">値</span><span class="sxs-lookup"><span data-stu-id="8499a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8499a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8499a-123">Authorization</span></span>|<span data-ttu-id="8499a-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8499a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8499a-125">承諾</span><span class="sxs-lookup"><span data-stu-id="8499a-125">Accept</span></span>|<span data-ttu-id="8499a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8499a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8499a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8499a-127">Request body</span></span>
<span data-ttu-id="8499a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8499a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8499a-129">応答</span><span class="sxs-lookup"><span data-stu-id="8499a-129">Response</span></span>
<span data-ttu-id="8499a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8499a-130">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8499a-131">例</span><span class="sxs-lookup"><span data-stu-id="8499a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8499a-132">要求</span><span class="sxs-lookup"><span data-stu-id="8499a-132">Request</span></span>
<span data-ttu-id="8499a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8499a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8499a-134">応答</span><span class="sxs-lookup"><span data-stu-id="8499a-134">Response</span></span>
<span data-ttu-id="8499a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8499a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
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
}
```



