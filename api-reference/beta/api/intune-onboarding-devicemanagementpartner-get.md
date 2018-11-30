---
title: Get deviceManagementPartner
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: f00ebc9e7452ecb12a2ec0512b07cba23d559bb6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071222"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="dce86-103">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="dce86-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="dce86-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dce86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dce86-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dce86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dce86-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dce86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dce86-107">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dce86-107">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dce86-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dce86-108">Prerequisites</span></span>
<span data-ttu-id="dce86-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dce86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dce86-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dce86-111">Permission type</span></span>|<span data-ttu-id="dce86-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dce86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dce86-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dce86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dce86-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dce86-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dce86-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dce86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dce86-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dce86-116">Not supported.</span></span>|
|<span data-ttu-id="dce86-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dce86-117">Application</span></span>|<span data-ttu-id="dce86-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dce86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dce86-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dce86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dce86-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dce86-120">Optional query parameters</span></span>
<span data-ttu-id="dce86-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dce86-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dce86-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dce86-122">Request headers</span></span>
|<span data-ttu-id="dce86-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dce86-123">Header</span></span>|<span data-ttu-id="dce86-124">値</span><span class="sxs-lookup"><span data-stu-id="dce86-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dce86-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dce86-125">Authorization</span></span>|<span data-ttu-id="dce86-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dce86-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dce86-127">Accept</span><span class="sxs-lookup"><span data-stu-id="dce86-127">Accept</span></span>|<span data-ttu-id="dce86-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dce86-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce86-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="dce86-129">Request body</span></span>
<span data-ttu-id="dce86-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dce86-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dce86-131">応答</span><span class="sxs-lookup"><span data-stu-id="dce86-131">Response</span></span>
<span data-ttu-id="dce86-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dce86-132">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce86-133">例</span><span class="sxs-lookup"><span data-stu-id="dce86-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="dce86-134">要求</span><span class="sxs-lookup"><span data-stu-id="dce86-134">Request</span></span>
<span data-ttu-id="dce86-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dce86-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="dce86-136">応答</span><span class="sxs-lookup"><span data-stu-id="dce86-136">Response</span></span>
<span data-ttu-id="dce86-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dce86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```





