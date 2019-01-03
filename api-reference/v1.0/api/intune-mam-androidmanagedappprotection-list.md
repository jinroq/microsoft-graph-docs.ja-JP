---
title: androidManagedAppProtections のリスト
description: androidManagedAppProtection オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 00b2ffe54aaeb37087520210386b00821882c8e7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317361"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="9a557-103">androidManagedAppProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="9a557-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="9a557-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a557-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a557-105">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9a557-105">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a557-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a557-106">Prerequisites</span></span>
<span data-ttu-id="9a557-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a557-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a557-109">Permission type</span></span>|<span data-ttu-id="9a557-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a557-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a557-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a557-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a557-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a557-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9a557-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a557-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a557-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a557-114">Not supported.</span></span>|
|<span data-ttu-id="9a557-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a557-115">Application</span></span>|<span data-ttu-id="9a557-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a557-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a557-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a557-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="9a557-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a557-118">Request headers</span></span>
|<span data-ttu-id="9a557-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a557-119">Header</span></span>|<span data-ttu-id="9a557-120">値</span><span class="sxs-lookup"><span data-stu-id="9a557-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a557-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a557-121">Authorization</span></span>|<span data-ttu-id="9a557-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9a557-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a557-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9a557-123">Accept</span></span>|<span data-ttu-id="9a557-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a557-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a557-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a557-125">Request body</span></span>
<span data-ttu-id="9a557-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a557-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a557-127">応答</span><span class="sxs-lookup"><span data-stu-id="9a557-127">Response</span></span>
<span data-ttu-id="9a557-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9a557-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a557-129">例</span><span class="sxs-lookup"><span data-stu-id="9a557-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a557-130">要求</span><span class="sxs-lookup"><span data-stu-id="9a557-130">Request</span></span>
<span data-ttu-id="9a557-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a557-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="9a557-132">応答</span><span class="sxs-lookup"><span data-stu-id="9a557-132">Response</span></span>
<span data-ttu-id="9a557-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a557-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
    }
  ]
}
```


