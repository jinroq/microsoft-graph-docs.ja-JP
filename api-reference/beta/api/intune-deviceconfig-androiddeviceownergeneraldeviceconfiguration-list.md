---
title: List androiddeviceowner一般 deviceconfigurん
description: androiddeviceownerのオブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38bdfd3c9db2b5b0a7a4f3e29fc908fd2f2b08c4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805678"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="ae6f9-103">List androiddeviceowner一般 deviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="ae6f9-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="ae6f9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae6f9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae6f9-106">[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-106">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae6f9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae6f9-107">Prerequisites</span></span>
<span data-ttu-id="ae6f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6f9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae6f9-110">Permission type</span></span>|<span data-ttu-id="ae6f9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae6f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae6f9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae6f9-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6f9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ae6f9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae6f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-115">Not supported.</span></span>|
|<span data-ttu-id="ae6f9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae6f9-116">Application</span></span>|<span data-ttu-id="ae6f9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae6f9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae6f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ae6f9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6f9-119">Request headers</span></span>
|<span data-ttu-id="ae6f9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6f9-120">Header</span></span>|<span data-ttu-id="ae6f9-121">値</span><span class="sxs-lookup"><span data-stu-id="ae6f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae6f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6f9-122">Authorization</span></span>|<span data-ttu-id="ae6f9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae6f9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae6f9-124">Accept</span></span>|<span data-ttu-id="ae6f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae6f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6f9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae6f9-126">Request body</span></span>
<span data-ttu-id="ae6f9-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae6f9-128">応答</span><span class="sxs-lookup"><span data-stu-id="ae6f9-128">Response</span></span>
<span data-ttu-id="ae6f9-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6f9-130">例</span><span class="sxs-lookup"><span data-stu-id="ae6f9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae6f9-131">要求</span><span class="sxs-lookup"><span data-stu-id="ae6f9-131">Request</span></span>
<span data-ttu-id="ae6f9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ae6f9-133">応答</span><span class="sxs-lookup"><span data-stu-id="ae6f9-133">Response</span></span>
<span data-ttu-id="ae6f9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3438

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountsBlockModification": true,
      "appsAllowInstallFromUnknownSources": true,
      "appsAutoUpdatePolicy": "userChoice",
      "appsDefaultPermissionPolicy": "prompt",
      "appsRecommendSkippingFirstUseHints": true,
      "bluetoothBlockConfiguration": true,
      "bluetoothBlockContactSharing": true,
      "cameraBlocked": true,
      "cellularBlockWiFiTethering": true,
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
      "kioskModeExitCode": "Kiosk Mode Exit Code value",
      "kioskModeVirtualHomeButtonEnabled": true,
      "kioskModeBluetoothConfigurationEnabled": true,
      "kioskModeWiFiConfigurationEnabled": true,
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordBlockKeyguardFeatures": [
        "camera"
      ],
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumLetterCharacters": 15,
      "passwordMinimumLowerCaseCharacters": 2,
      "passwordMinimumNonLetterCharacters": 2,
      "passwordMinimumNumericCharacters": 0,
      "passwordMinimumSymbolCharacters": 15,
      "passwordMinimumUpperCaseCharacters": 2,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "playStoreMode": "allowList",
      "safeBootBlocked": true,
      "screenCaptureBlocked": true,
      "securityAllowDebuggingFeatures": true,
      "securityRequireVerifyApps": true,
      "statusBarBlocked": true,
      "stayOnModes": [
        "ac"
      ],
      "storageAllowUsb": true,
      "storageBlockExternalMedia": true,
      "storageBlockUsbFileTransfer": true,
      "systemUpdateWindowStartMinutesAfterMidnight": 11,
      "systemUpdateWindowEndMinutesAfterMidnight": 9,
      "systemUpdateInstallType": "postpone",
      "systemWindowsBlocked": true,
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnAlwaysOnLockdownMode": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```





