---
title: Get windowsPhone81CompliancePolicy
description: windowsPhone81CompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 282a70a78178b3cd7df2d018248f9c2da5fc2389
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358276"
---
# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="a23b0-103">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a23b0-103">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="a23b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a23b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a23b0-105">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a23b0-105">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a23b0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a23b0-106">Prerequisites</span></span>
<span data-ttu-id="a23b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a23b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a23b0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a23b0-109">Permission type</span></span>|<span data-ttu-id="a23b0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a23b0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a23b0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a23b0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a23b0-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a23b0-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a23b0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a23b0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a23b0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a23b0-114">Not supported.</span></span>|
|<span data-ttu-id="a23b0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a23b0-115">Application</span></span>|<span data-ttu-id="a23b0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a23b0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a23b0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a23b0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a23b0-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a23b0-118">Optional query parameters</span></span>
<span data-ttu-id="a23b0-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a23b0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a23b0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a23b0-120">Request headers</span></span>
|<span data-ttu-id="a23b0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a23b0-121">Header</span></span>|<span data-ttu-id="a23b0-122">値</span><span class="sxs-lookup"><span data-stu-id="a23b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a23b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a23b0-123">Authorization</span></span>|<span data-ttu-id="a23b0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a23b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a23b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a23b0-125">Accept</span></span>|<span data-ttu-id="a23b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a23b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a23b0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a23b0-127">Request body</span></span>
<span data-ttu-id="a23b0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a23b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a23b0-129">応答</span><span class="sxs-lookup"><span data-stu-id="a23b0-129">Response</span></span>
<span data-ttu-id="a23b0-130">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a23b0-130">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a23b0-131">例</span><span class="sxs-lookup"><span data-stu-id="a23b0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a23b0-132">要求</span><span class="sxs-lookup"><span data-stu-id="a23b0-132">Request</span></span>
<span data-ttu-id="a23b0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a23b0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a23b0-134">応答</span><span class="sxs-lookup"><span data-stu-id="a23b0-134">Response</span></span>
<span data-ttu-id="a23b0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a23b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```


