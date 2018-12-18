---
title: targetedManagedAppProtection の取得
description: targetedManagedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: c8612f46f1a5672b4ca3dd2f1b1d90703a5b7aad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343912"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="357b8-103">targetedManagedAppProtection の取得</span><span class="sxs-lookup"><span data-stu-id="357b8-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="357b8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="357b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="357b8-105">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="357b8-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="357b8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="357b8-106">Prerequisites</span></span>
<span data-ttu-id="357b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="357b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357b8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="357b8-109">Permission type</span></span>|<span data-ttu-id="357b8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="357b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="357b8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="357b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="357b8-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="357b8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="357b8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="357b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="357b8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="357b8-114">Not supported.</span></span>|
|<span data-ttu-id="357b8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="357b8-115">Application</span></span>|<span data-ttu-id="357b8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="357b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="357b8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="357b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="357b8-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="357b8-118">Optional query parameters</span></span>
<span data-ttu-id="357b8-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="357b8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="357b8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="357b8-120">Request headers</span></span>
|<span data-ttu-id="357b8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="357b8-121">Header</span></span>|<span data-ttu-id="357b8-122">値</span><span class="sxs-lookup"><span data-stu-id="357b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="357b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="357b8-123">Authorization</span></span>|<span data-ttu-id="357b8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="357b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="357b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="357b8-125">Accept</span></span>|<span data-ttu-id="357b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="357b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="357b8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="357b8-127">Request body</span></span>
<span data-ttu-id="357b8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="357b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="357b8-129">応答</span><span class="sxs-lookup"><span data-stu-id="357b8-129">Response</span></span>
<span data-ttu-id="357b8-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="357b8-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="357b8-131">例</span><span class="sxs-lookup"><span data-stu-id="357b8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="357b8-132">要求</span><span class="sxs-lookup"><span data-stu-id="357b8-132">Request</span></span>
<span data-ttu-id="357b8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="357b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="357b8-134">応答</span><span class="sxs-lookup"><span data-stu-id="357b8-134">Response</span></span>
<span data-ttu-id="357b8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="357b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
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
    "isAssigned": true
  }
}
```



