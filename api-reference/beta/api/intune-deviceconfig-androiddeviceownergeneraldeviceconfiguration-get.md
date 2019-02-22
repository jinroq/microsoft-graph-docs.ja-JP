---
title: androiddeviceowner一般の devic/デバイスを取得する
description: androiddeviceownerのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24664d4322f95b8f2212cff95232978e6db9ad7f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168279"
---
# <a name="get-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="e0aae-103">androiddeviceowner一般の devic/デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="e0aae-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e0aae-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0aae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0aae-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0aae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0aae-106">[androiddeviceownerの](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)プロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e0aae-106">Read properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0aae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0aae-107">Prerequisites</span></span>
<span data-ttu-id="e0aae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e0aae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0aae-110">Permission type</span></span>|<span data-ttu-id="e0aae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0aae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0aae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0aae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0aae-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0aae-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e0aae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0aae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0aae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0aae-115">Not supported.</span></span>|
|<span data-ttu-id="e0aae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0aae-116">Application</span></span>|<span data-ttu-id="e0aae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0aae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0aae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0aae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0aae-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e0aae-119">Optional query parameters</span></span>
<span data-ttu-id="e0aae-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e0aae-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0aae-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0aae-121">Request headers</span></span>
|<span data-ttu-id="e0aae-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0aae-122">Header</span></span>|<span data-ttu-id="e0aae-123">値</span><span class="sxs-lookup"><span data-stu-id="e0aae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0aae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0aae-124">Authorization</span></span>|<span data-ttu-id="e0aae-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e0aae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0aae-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e0aae-126">Accept</span></span>|<span data-ttu-id="e0aae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e0aae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0aae-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0aae-128">Request body</span></span>
<span data-ttu-id="e0aae-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e0aae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0aae-130">応答</span><span class="sxs-lookup"><span data-stu-id="e0aae-130">Response</span></span>
<span data-ttu-id="e0aae-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androiddeviceowner一般](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)の devic/オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0aae-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0aae-132">例</span><span class="sxs-lookup"><span data-stu-id="e0aae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0aae-133">要求</span><span class="sxs-lookup"><span data-stu-id="e0aae-133">Request</span></span>
<span data-ttu-id="e0aae-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0aae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e0aae-135">応答</span><span class="sxs-lookup"><span data-stu-id="e0aae-135">Response</span></span>
<span data-ttu-id="e0aae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0aae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2854

{
  "value": {
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
    "microphoneForceMute": true,
    "networkEscapeHatchAllowed": true,
    "nfcBlockOutgoingBeam": true,
    "passwordBlockKeyguard": true,
    "passwordBlockKeyguardFeatures": [
      "camera"
    ],
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordCountToBlock": 4,
    "passwordRequiredType": "required",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
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
}
```




