---
title: Get iosCompliancePolicy
description: iosCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccb4ee75266e85f5089b17ec8670572cbfe3cfc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467583"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="c3437-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c3437-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="c3437-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3437-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3437-106">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c3437-106">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3437-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3437-107">Prerequisites</span></span>
<span data-ttu-id="c3437-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3437-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3437-110">Permission type</span></span>|<span data-ttu-id="c3437-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3437-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3437-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3437-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3437-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3437-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c3437-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3437-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3437-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3437-115">Not supported.</span></span>|
|<span data-ttu-id="c3437-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3437-116">Application</span></span>|<span data-ttu-id="c3437-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3437-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3437-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3437-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3437-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3437-119">Optional query parameters</span></span>
<span data-ttu-id="c3437-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3437-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3437-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3437-121">Request headers</span></span>
|<span data-ttu-id="c3437-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3437-122">Header</span></span>|<span data-ttu-id="c3437-123">値</span><span class="sxs-lookup"><span data-stu-id="c3437-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3437-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3437-124">Authorization</span></span>|<span data-ttu-id="c3437-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3437-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3437-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c3437-126">Accept</span></span>|<span data-ttu-id="c3437-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c3437-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3437-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3437-128">Request body</span></span>
<span data-ttu-id="c3437-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3437-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3437-130">応答</span><span class="sxs-lookup"><span data-stu-id="c3437-130">Response</span></span>
<span data-ttu-id="c3437-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3437-131">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3437-132">例</span><span class="sxs-lookup"><span data-stu-id="c3437-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3437-133">要求</span><span class="sxs-lookup"><span data-stu-id="c3437-133">Request</span></span>
<span data-ttu-id="c3437-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3437-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="c3437-135">応答</span><span class="sxs-lookup"><span data-stu-id="c3437-135">Response</span></span>
<span data-ttu-id="c3437-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3437-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1504

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "osMinimumBuildVersion": "Os Minimum Build Version value",
    "osMaximumBuildVersion": "Os Maximum Build Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true,
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
}
```





