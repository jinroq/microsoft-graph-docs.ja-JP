---
title: AndroidWorkProfileCompliancePolicy を取得する
description: AndroidWorkProfileCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5291c9844eebc19b4030c129fdc9887f84015cee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019577"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="5fc01-103">AndroidWorkProfileCompliancePolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="5fc01-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="5fc01-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5fc01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fc01-105">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5fc01-105">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fc01-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="5fc01-106">Prerequisites</span></span>
<span data-ttu-id="5fc01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5fc01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc01-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5fc01-109">Permission type</span></span>|<span data-ttu-id="5fc01-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5fc01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fc01-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5fc01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fc01-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fc01-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5fc01-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5fc01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fc01-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fc01-114">Not supported.</span></span>|
|<span data-ttu-id="5fc01-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5fc01-115">Application</span></span>|<span data-ttu-id="5fc01-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fc01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fc01-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5fc01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fc01-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5fc01-118">Optional query parameters</span></span>
<span data-ttu-id="5fc01-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5fc01-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fc01-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fc01-120">Request headers</span></span>
|<span data-ttu-id="5fc01-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fc01-121">Header</span></span>|<span data-ttu-id="5fc01-122">値</span><span class="sxs-lookup"><span data-stu-id="5fc01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fc01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fc01-123">Authorization</span></span>|<span data-ttu-id="5fc01-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5fc01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fc01-125">承諾</span><span class="sxs-lookup"><span data-stu-id="5fc01-125">Accept</span></span>|<span data-ttu-id="5fc01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fc01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fc01-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5fc01-127">Request body</span></span>
<span data-ttu-id="5fc01-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5fc01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fc01-129">応答</span><span class="sxs-lookup"><span data-stu-id="5fc01-129">Response</span></span>
<span data-ttu-id="5fc01-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5fc01-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fc01-131">例</span><span class="sxs-lookup"><span data-stu-id="5fc01-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fc01-132">要求</span><span class="sxs-lookup"><span data-stu-id="5fc01-132">Request</span></span>
<span data-ttu-id="5fc01-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5fc01-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="5fc01-134">応答</span><span class="sxs-lookup"><span data-stu-id="5fc01-134">Response</span></span>
<span data-ttu-id="5fc01-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5fc01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1417

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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



