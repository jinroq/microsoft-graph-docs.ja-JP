---
title: Get windows10CompliancePolicy
description: windows10CompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 58208e40cba356cec312d07bf98e945a2ef4ebf6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307967"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="2dc88-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2dc88-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="2dc88-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2dc88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dc88-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dc88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2dc88-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dc88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dc88-107">[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2dc88-107">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2dc88-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2dc88-108">Prerequisites</span></span>
<span data-ttu-id="2dc88-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dc88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dc88-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2dc88-111">Permission type</span></span>|<span data-ttu-id="2dc88-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2dc88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dc88-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2dc88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2dc88-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2dc88-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2dc88-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2dc88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dc88-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dc88-116">Not supported.</span></span>|
|<span data-ttu-id="2dc88-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2dc88-117">Application</span></span>|<span data-ttu-id="2dc88-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dc88-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dc88-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2dc88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2dc88-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2dc88-120">Optional query parameters</span></span>
<span data-ttu-id="2dc88-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2dc88-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2dc88-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dc88-122">Request headers</span></span>
|<span data-ttu-id="2dc88-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dc88-123">Header</span></span>|<span data-ttu-id="2dc88-124">値</span><span class="sxs-lookup"><span data-stu-id="2dc88-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dc88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dc88-125">Authorization</span></span>|<span data-ttu-id="2dc88-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2dc88-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dc88-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2dc88-127">Accept</span></span>|<span data-ttu-id="2dc88-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2dc88-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dc88-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2dc88-129">Request body</span></span>
<span data-ttu-id="2dc88-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2dc88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dc88-131">応答</span><span class="sxs-lookup"><span data-stu-id="2dc88-131">Response</span></span>
<span data-ttu-id="2dc88-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2dc88-132">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dc88-133">例</span><span class="sxs-lookup"><span data-stu-id="2dc88-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2dc88-134">要求</span><span class="sxs-lookup"><span data-stu-id="2dc88-134">Request</span></span>
<span data-ttu-id="2dc88-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2dc88-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="2dc88-136">応答</span><span class="sxs-lookup"><span data-stu-id="2dc88-136">Response</span></span>
<span data-ttu-id="2dc88-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2dc88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1951

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2919ae62-ae62-2919-62ae-192962ae1929",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordRequiredToUnlockFromIdle": true,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "requireHealthyDeviceReport": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
    "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "defenderEnabled": true,
    "defenderVersion": "Defender Version value",
    "signatureOutOfDate": true,
    "rtpEnabled": true,
    "antivirusRequired": true,
    "antiSpywareRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ],
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "configurationManagerComplianceRequired": true
  }
}
```




