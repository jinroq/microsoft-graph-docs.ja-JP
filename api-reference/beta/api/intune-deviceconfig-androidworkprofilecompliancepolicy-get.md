---
title: AndroidWorkProfileCompliancePolicy を取得する
description: AndroidWorkProfileCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5773d37839a9160afe948001b19f3024653d382
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969653"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="7b207-103">AndroidWorkProfileCompliancePolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="7b207-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="7b207-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b207-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b207-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b207-106">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7b207-106">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b207-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7b207-107">Prerequisites</span></span>
<span data-ttu-id="7b207-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b207-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b207-110">Permission type</span></span>|<span data-ttu-id="7b207-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7b207-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b207-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b207-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b207-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b207-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b207-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b207-115">Not supported.</span></span>|
|<span data-ttu-id="7b207-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b207-116">Application</span></span>|<span data-ttu-id="7b207-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b207-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b207-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b207-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b207-119">Optional query parameters</span></span>
<span data-ttu-id="7b207-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7b207-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b207-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b207-121">Request headers</span></span>
|<span data-ttu-id="7b207-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b207-122">Header</span></span>|<span data-ttu-id="7b207-123">値</span><span class="sxs-lookup"><span data-stu-id="7b207-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b207-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b207-124">Authorization</span></span>|<span data-ttu-id="7b207-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b207-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b207-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7b207-126">Accept</span></span>|<span data-ttu-id="7b207-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7b207-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b207-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b207-128">Request body</span></span>
<span data-ttu-id="7b207-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7b207-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b207-130">応答</span><span class="sxs-lookup"><span data-stu-id="7b207-130">Response</span></span>
<span data-ttu-id="7b207-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7b207-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b207-132">例</span><span class="sxs-lookup"><span data-stu-id="7b207-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b207-133">要求</span><span class="sxs-lookup"><span data-stu-id="7b207-133">Request</span></span>
<span data-ttu-id="7b207-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7b207-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="7b207-135">応答</span><span class="sxs-lookup"><span data-stu-id="7b207-135">Response</span></span>
<span data-ttu-id="7b207-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7b207-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1542

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4e385271-5271-4e38-7152-384e7152384e",
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
    "securityRequireCompanyPortalAppIntegrity": true
  }
}
```





