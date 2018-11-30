---
title: AndroidWorkProfileCompliancePolicy を取得します。
description: AndroidWorkProfileCompliancePolicy オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: cc4724968280201c883f7d6016caaeecc8910628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023364"
---
# <a name="get-androidworkprofilecompliancepolicy"></a><span data-ttu-id="e9dac-103">AndroidWorkProfileCompliancePolicy を取得します。</span><span class="sxs-lookup"><span data-stu-id="e9dac-103">Get androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="e9dac-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e9dac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9dac-105">[AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9dac-105">Read properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9dac-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e9dac-106">Prerequisites</span></span>
<span data-ttu-id="e9dac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9dac-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9dac-109">Permission type</span></span>|<span data-ttu-id="e9dac-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9dac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9dac-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9dac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9dac-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9dac-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e9dac-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9dac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9dac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9dac-114">Not supported.</span></span>|
|<span data-ttu-id="e9dac-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9dac-115">Application</span></span>|<span data-ttu-id="e9dac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9dac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9dac-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9dac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9dac-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9dac-118">Optional query parameters</span></span>
<span data-ttu-id="e9dac-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e9dac-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9dac-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9dac-120">Request headers</span></span>
|<span data-ttu-id="e9dac-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9dac-121">Header</span></span>|<span data-ttu-id="e9dac-122">値</span><span class="sxs-lookup"><span data-stu-id="e9dac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9dac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9dac-123">Authorization</span></span>|<span data-ttu-id="e9dac-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e9dac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9dac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9dac-125">Accept</span></span>|<span data-ttu-id="e9dac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9dac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9dac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9dac-127">Request body</span></span>
<span data-ttu-id="e9dac-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e9dac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9dac-129">応答</span><span class="sxs-lookup"><span data-stu-id="e9dac-129">Response</span></span>
<span data-ttu-id="e9dac-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e9dac-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9dac-131">例</span><span class="sxs-lookup"><span data-stu-id="e9dac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9dac-132">要求</span><span class="sxs-lookup"><span data-stu-id="e9dac-132">Request</span></span>
<span data-ttu-id="e9dac-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e9dac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="e9dac-134">応答</span><span class="sxs-lookup"><span data-stu-id="e9dac-134">Response</span></span>
<span data-ttu-id="e9dac-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e9dac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



