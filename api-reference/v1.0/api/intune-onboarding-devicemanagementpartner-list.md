---
title: deviceManagementPartners のリスト
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: c308dc378fdcd0257b72b4a5948635ec0c1fa257
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021018"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="67008-103">deviceManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="67008-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="67008-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67008-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67008-105">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="67008-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67008-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="67008-106">Prerequisites</span></span>
<span data-ttu-id="67008-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67008-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67008-109">Permission type</span></span>|<span data-ttu-id="67008-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67008-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67008-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67008-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67008-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="67008-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="67008-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67008-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67008-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67008-114">Not supported.</span></span>|
|<span data-ttu-id="67008-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67008-115">Application</span></span>|<span data-ttu-id="67008-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67008-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67008-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67008-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="67008-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67008-118">Request headers</span></span>
|<span data-ttu-id="67008-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67008-119">Header</span></span>|<span data-ttu-id="67008-120">値</span><span class="sxs-lookup"><span data-stu-id="67008-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67008-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67008-121">Authorization</span></span>|<span data-ttu-id="67008-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67008-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67008-123">Accept</span><span class="sxs-lookup"><span data-stu-id="67008-123">Accept</span></span>|<span data-ttu-id="67008-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67008-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67008-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67008-125">Request body</span></span>
<span data-ttu-id="67008-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67008-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67008-127">応答</span><span class="sxs-lookup"><span data-stu-id="67008-127">Response</span></span>
<span data-ttu-id="67008-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="67008-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67008-129">例</span><span class="sxs-lookup"><span data-stu-id="67008-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="67008-130">要求</span><span class="sxs-lookup"><span data-stu-id="67008-130">Request</span></span>
<span data-ttu-id="67008-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67008-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="67008-132">応答</span><span class="sxs-lookup"><span data-stu-id="67008-132">Response</span></span>
<span data-ttu-id="67008-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67008-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```



