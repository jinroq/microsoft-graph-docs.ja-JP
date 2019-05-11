---
title: androidCompliancePolicies のリスト
description: androidCompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f592c36763a3e99c8dc1d46330b5a3ff508e59f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933299"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="71efc-103">androidCompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="71efc-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="71efc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71efc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71efc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71efc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71efc-106">[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="71efc-106">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71efc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="71efc-107">Prerequisites</span></span>
<span data-ttu-id="71efc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71efc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71efc-110">Permission type</span></span>|<span data-ttu-id="71efc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71efc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71efc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71efc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71efc-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71efc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71efc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71efc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71efc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71efc-115">Not supported.</span></span>|
|<span data-ttu-id="71efc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71efc-116">Application</span></span>|<span data-ttu-id="71efc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71efc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71efc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71efc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="71efc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71efc-119">Request headers</span></span>
|<span data-ttu-id="71efc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71efc-120">Header</span></span>|<span data-ttu-id="71efc-121">値</span><span class="sxs-lookup"><span data-stu-id="71efc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71efc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71efc-122">Authorization</span></span>|<span data-ttu-id="71efc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="71efc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71efc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="71efc-124">Accept</span></span>|<span data-ttu-id="71efc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71efc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71efc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71efc-126">Request body</span></span>
<span data-ttu-id="71efc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71efc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71efc-128">応答</span><span class="sxs-lookup"><span data-stu-id="71efc-128">Response</span></span>
<span data-ttu-id="71efc-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="71efc-129">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71efc-130">例</span><span class="sxs-lookup"><span data-stu-id="71efc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71efc-131">要求</span><span class="sxs-lookup"><span data-stu-id="71efc-131">Request</span></span>
<span data-ttu-id="71efc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71efc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="71efc-133">応答</span><span class="sxs-lookup"><span data-stu-id="71efc-133">Response</span></span>
<span data-ttu-id="71efc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71efc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1961

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true,
      "conditionStatementId": "Condition Statement Id value",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```




