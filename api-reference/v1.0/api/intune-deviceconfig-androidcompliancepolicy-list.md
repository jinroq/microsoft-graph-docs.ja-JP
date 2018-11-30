---
title: androidCompliancePolicies のリスト
description: androidCompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 289529aaa56e55b5a6c66fd1335ceaa8e8e565df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021234"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="41a87-103">androidCompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="41a87-103">List androidCompliancePolicies</span></span>

> <span data-ttu-id="41a87-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="41a87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41a87-105">[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="41a87-105">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41a87-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="41a87-106">Prerequisites</span></span>
<span data-ttu-id="41a87-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41a87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41a87-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41a87-109">Permission type</span></span>|<span data-ttu-id="41a87-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41a87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41a87-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41a87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41a87-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41a87-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41a87-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41a87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41a87-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41a87-114">Not supported.</span></span>|
|<span data-ttu-id="41a87-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41a87-115">Application</span></span>|<span data-ttu-id="41a87-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41a87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41a87-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41a87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="41a87-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41a87-118">Request headers</span></span>
|<span data-ttu-id="41a87-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41a87-119">Header</span></span>|<span data-ttu-id="41a87-120">値</span><span class="sxs-lookup"><span data-stu-id="41a87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41a87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41a87-121">Authorization</span></span>|<span data-ttu-id="41a87-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="41a87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41a87-123">Accept</span><span class="sxs-lookup"><span data-stu-id="41a87-123">Accept</span></span>|<span data-ttu-id="41a87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41a87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41a87-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="41a87-125">Request body</span></span>
<span data-ttu-id="41a87-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41a87-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41a87-127">応答</span><span class="sxs-lookup"><span data-stu-id="41a87-127">Response</span></span>
<span data-ttu-id="41a87-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="41a87-128">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41a87-129">例</span><span class="sxs-lookup"><span data-stu-id="41a87-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="41a87-130">要求</span><span class="sxs-lookup"><span data-stu-id="41a87-130">Request</span></span>
<span data-ttu-id="41a87-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41a87-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="41a87-132">応答</span><span class="sxs-lookup"><span data-stu-id="41a87-132">Response</span></span>
<span data-ttu-id="41a87-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41a87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```



