---
title: managedAppProtections のリスト
description: managedAppProtection オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed611086d0bdc52e0247104863238c025a1974b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403925"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="18411-103">managedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="18411-103">List managedAppProtections</span></span>

> <span data-ttu-id="18411-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18411-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18411-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18411-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18411-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18411-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18411-107">[managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="18411-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18411-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="18411-108">Prerequisites</span></span>
<span data-ttu-id="18411-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18411-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18411-111">Permission type</span></span>|<span data-ttu-id="18411-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18411-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18411-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18411-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18411-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18411-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="18411-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18411-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18411-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18411-116">Not supported.</span></span>|
|<span data-ttu-id="18411-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18411-117">Application</span></span>|<span data-ttu-id="18411-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18411-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18411-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18411-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="18411-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18411-120">Request headers</span></span>
|<span data-ttu-id="18411-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18411-121">Header</span></span>|<span data-ttu-id="18411-122">値</span><span class="sxs-lookup"><span data-stu-id="18411-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18411-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18411-123">Authorization</span></span>|<span data-ttu-id="18411-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18411-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18411-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18411-125">Accept</span></span>|<span data-ttu-id="18411-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18411-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18411-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18411-127">Request body</span></span>
<span data-ttu-id="18411-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18411-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18411-129">応答</span><span class="sxs-lookup"><span data-stu-id="18411-129">Response</span></span>
<span data-ttu-id="18411-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="18411-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18411-131">例</span><span class="sxs-lookup"><span data-stu-id="18411-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18411-132">要求</span><span class="sxs-lookup"><span data-stu-id="18411-132">Request</span></span>
<span data-ttu-id="18411-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18411-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="18411-134">応答</span><span class="sxs-lookup"><span data-stu-id="18411-134">Response</span></span>
<span data-ttu-id="18411-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18411-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2094

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S"
    }
  ]
}
```




