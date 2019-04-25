---
title: Get managedAppProtection
description: managedAppProtection オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c0c03051fc785c4bac4e908198fda359c30971
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529724"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="f2e62-103">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="f2e62-103">Get managedAppProtection</span></span>

> <span data-ttu-id="f2e62-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2e62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2e62-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2e62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e62-106">[managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2e62-106">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2e62-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2e62-107">Prerequisites</span></span>
<span data-ttu-id="f2e62-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e62-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2e62-110">Permission type</span></span>|<span data-ttu-id="f2e62-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2e62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e62-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2e62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e62-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2e62-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2e62-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2e62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2e62-115">Not supported.</span></span>|
|<span data-ttu-id="f2e62-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2e62-116">Application</span></span>|<span data-ttu-id="f2e62-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2e62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e62-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2e62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2e62-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2e62-119">Optional query parameters</span></span>
<span data-ttu-id="f2e62-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f2e62-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2e62-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2e62-121">Request headers</span></span>
|<span data-ttu-id="f2e62-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2e62-122">Header</span></span>|<span data-ttu-id="f2e62-123">値</span><span class="sxs-lookup"><span data-stu-id="f2e62-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e62-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e62-124">Authorization</span></span>|<span data-ttu-id="f2e62-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2e62-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e62-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f2e62-126">Accept</span></span>|<span data-ttu-id="f2e62-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e62-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e62-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2e62-128">Request body</span></span>
<span data-ttu-id="f2e62-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2e62-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2e62-130">応答</span><span class="sxs-lookup"><span data-stu-id="f2e62-130">Response</span></span>
<span data-ttu-id="f2e62-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2e62-131">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e62-132">例</span><span class="sxs-lookup"><span data-stu-id="f2e62-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2e62-133">要求</span><span class="sxs-lookup"><span data-stu-id="f2e62-133">Request</span></span>
<span data-ttu-id="f2e62-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2e62-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="f2e62-135">応答</span><span class="sxs-lookup"><span data-stu-id="f2e62-135">Response</span></span>
<span data-ttu-id="f2e62-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2e62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2053

{
  "value": {
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
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14
  }
}
```





