---
title: Get windows10CompliancePolicy
description: windows10CompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe32502087a729cb82d51a583431eb52af6c6474
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946181"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="7f502-103">Get windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7f502-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="7f502-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f502-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f502-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f502-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f502-106">[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f502-106">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f502-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f502-107">Prerequisites</span></span>
<span data-ttu-id="7f502-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f502-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f502-110">Permission type</span></span>|<span data-ttu-id="7f502-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f502-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f502-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f502-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f502-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f502-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f502-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f502-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f502-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f502-115">Not supported.</span></span>|
|<span data-ttu-id="7f502-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f502-116">Application</span></span>|<span data-ttu-id="7f502-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f502-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f502-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f502-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f502-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f502-119">Optional query parameters</span></span>
<span data-ttu-id="7f502-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f502-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f502-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f502-121">Request headers</span></span>
|<span data-ttu-id="7f502-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f502-122">Header</span></span>|<span data-ttu-id="7f502-123">値</span><span class="sxs-lookup"><span data-stu-id="7f502-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f502-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f502-124">Authorization</span></span>|<span data-ttu-id="7f502-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f502-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f502-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7f502-126">Accept</span></span>|<span data-ttu-id="7f502-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7f502-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f502-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f502-128">Request body</span></span>
<span data-ttu-id="7f502-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f502-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f502-130">応答</span><span class="sxs-lookup"><span data-stu-id="7f502-130">Response</span></span>
<span data-ttu-id="7f502-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f502-131">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f502-132">例</span><span class="sxs-lookup"><span data-stu-id="7f502-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f502-133">要求</span><span class="sxs-lookup"><span data-stu-id="7f502-133">Request</span></span>
<span data-ttu-id="7f502-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f502-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="7f502-135">応答</span><span class="sxs-lookup"><span data-stu-id="7f502-135">Response</span></span>
<span data-ttu-id="7f502-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f502-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

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
    "configurationManagerComplianceRequired": true,
    "tpmRequired": true
  }
}
```





