---
title: Get iosCompliancePolicy
description: iosCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 8dea39098e36cc384c366aec4c110140b8aa9bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021098"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="79242-103">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="79242-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="79242-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79242-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79242-105">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="79242-105">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79242-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="79242-106">Prerequisites</span></span>
<span data-ttu-id="79242-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79242-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79242-109">Permission type</span></span>|<span data-ttu-id="79242-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79242-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79242-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79242-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79242-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79242-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79242-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79242-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79242-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79242-114">Not supported.</span></span>|
|<span data-ttu-id="79242-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79242-115">Application</span></span>|<span data-ttu-id="79242-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79242-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79242-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79242-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79242-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79242-118">Optional query parameters</span></span>
<span data-ttu-id="79242-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79242-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="79242-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79242-120">Request headers</span></span>
|<span data-ttu-id="79242-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79242-121">Header</span></span>|<span data-ttu-id="79242-122">値</span><span class="sxs-lookup"><span data-stu-id="79242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79242-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79242-123">Authorization</span></span>|<span data-ttu-id="79242-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79242-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79242-125">Accept</span></span>|<span data-ttu-id="79242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79242-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79242-127">Request body</span></span>
<span data-ttu-id="79242-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79242-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79242-129">応答</span><span class="sxs-lookup"><span data-stu-id="79242-129">Response</span></span>
<span data-ttu-id="79242-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79242-130">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79242-131">例</span><span class="sxs-lookup"><span data-stu-id="79242-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="79242-132">要求</span><span class="sxs-lookup"><span data-stu-id="79242-132">Request</span></span>
<span data-ttu-id="79242-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79242-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="79242-134">応答</span><span class="sxs-lookup"><span data-stu-id="79242-134">Response</span></span>
<span data-ttu-id="79242-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79242-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 978

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
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
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true
  }
}
```



