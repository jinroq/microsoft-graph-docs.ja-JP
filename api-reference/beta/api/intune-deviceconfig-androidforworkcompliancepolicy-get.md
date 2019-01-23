---
title: AndroidForWorkCompliancePolicy を取得します。
description: AndroidForWorkCompliancePolicy オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6af08fc0c9453e2401036c1538b4be44e8d4f891
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413956"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="dbebd-103">AndroidForWorkCompliancePolicy を取得します。</span><span class="sxs-lookup"><span data-stu-id="dbebd-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="dbebd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dbebd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dbebd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbebd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbebd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dbebd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbebd-107">[AndroidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbebd-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbebd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dbebd-108">Prerequisites</span></span>
<span data-ttu-id="dbebd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbebd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dbebd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dbebd-111">Permission type</span></span>|<span data-ttu-id="dbebd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dbebd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbebd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dbebd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbebd-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbebd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbebd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbebd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbebd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbebd-116">Not supported.</span></span>|
|<span data-ttu-id="dbebd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dbebd-117">Application</span></span>|<span data-ttu-id="dbebd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbebd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbebd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dbebd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbebd-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dbebd-120">Optional query parameters</span></span>
<span data-ttu-id="dbebd-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dbebd-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbebd-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbebd-122">Request headers</span></span>
|<span data-ttu-id="dbebd-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbebd-123">Header</span></span>|<span data-ttu-id="dbebd-124">値</span><span class="sxs-lookup"><span data-stu-id="dbebd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbebd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbebd-125">Authorization</span></span>|<span data-ttu-id="dbebd-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dbebd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbebd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="dbebd-127">Accept</span></span>|<span data-ttu-id="dbebd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dbebd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbebd-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="dbebd-129">Request body</span></span>
<span data-ttu-id="dbebd-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dbebd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbebd-131">応答</span><span class="sxs-lookup"><span data-stu-id="dbebd-131">Response</span></span>
<span data-ttu-id="dbebd-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="dbebd-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbebd-133">例</span><span class="sxs-lookup"><span data-stu-id="dbebd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbebd-134">要求</span><span class="sxs-lookup"><span data-stu-id="dbebd-134">Request</span></span>
<span data-ttu-id="dbebd-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dbebd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="dbebd-136">応答</span><span class="sxs-lookup"><span data-stu-id="dbebd-136">Response</span></span>
<span data-ttu-id="dbebd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dbebd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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




