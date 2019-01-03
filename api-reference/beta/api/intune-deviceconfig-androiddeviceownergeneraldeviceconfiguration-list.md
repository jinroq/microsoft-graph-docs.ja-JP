---
title: リスト androidDeviceOwnerGeneralDeviceConfigurations
description: AndroidDeviceOwnerGeneralDeviceConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: ad0b8a59ae5db2b1feb38922b8eece9af8132301
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335715"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="3f264-103">リスト androidDeviceOwnerGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="3f264-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="3f264-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f264-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f264-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f264-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f264-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3f264-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f264-107">[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3f264-107">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f264-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f264-108">Prerequisites</span></span>
<span data-ttu-id="3f264-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f264-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f264-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f264-111">Permission type</span></span>|<span data-ttu-id="3f264-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f264-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f264-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f264-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f264-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f264-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3f264-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f264-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f264-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f264-116">Not supported.</span></span>|
|<span data-ttu-id="3f264-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f264-117">Application</span></span>|<span data-ttu-id="3f264-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f264-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f264-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f264-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f264-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f264-120">Request headers</span></span>
|<span data-ttu-id="3f264-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f264-121">Header</span></span>|<span data-ttu-id="3f264-122">値</span><span class="sxs-lookup"><span data-stu-id="3f264-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f264-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f264-123">Authorization</span></span>|<span data-ttu-id="3f264-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3f264-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f264-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f264-125">Accept</span></span>|<span data-ttu-id="3f264-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f264-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f264-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f264-127">Request body</span></span>
<span data-ttu-id="3f264-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3f264-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f264-129">応答</span><span class="sxs-lookup"><span data-stu-id="3f264-129">Response</span></span>
<span data-ttu-id="3f264-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3f264-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f264-131">例</span><span class="sxs-lookup"><span data-stu-id="3f264-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f264-132">要求</span><span class="sxs-lookup"><span data-stu-id="3f264-132">Request</span></span>
<span data-ttu-id="3f264-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f264-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3f264-134">応答</span><span class="sxs-lookup"><span data-stu-id="3f264-134">Response</span></span>
<span data-ttu-id="3f264-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f264-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2549

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
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
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
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```




