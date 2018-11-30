---
title: telecomExpenseManagementPartner の取得
description: telecomExpenseManagementPartner オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 4b0e33b86a084d97c426134f42e48711b646c86f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022758"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="679dc-103">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="679dc-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="679dc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="679dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="679dc-105">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="679dc-105">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="679dc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="679dc-106">Prerequisites</span></span>
<span data-ttu-id="679dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="679dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679dc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="679dc-109">Permission type</span></span>|<span data-ttu-id="679dc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="679dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="679dc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="679dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="679dc-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="679dc-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="679dc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="679dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="679dc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="679dc-114">Not supported.</span></span>|
|<span data-ttu-id="679dc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="679dc-115">Application</span></span>|<span data-ttu-id="679dc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="679dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="679dc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="679dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="679dc-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="679dc-118">Optional query parameters</span></span>
<span data-ttu-id="679dc-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="679dc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="679dc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="679dc-120">Request headers</span></span>
|<span data-ttu-id="679dc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="679dc-121">Header</span></span>|<span data-ttu-id="679dc-122">値</span><span class="sxs-lookup"><span data-stu-id="679dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="679dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="679dc-123">Authorization</span></span>|<span data-ttu-id="679dc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="679dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="679dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="679dc-125">Accept</span></span>|<span data-ttu-id="679dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="679dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="679dc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="679dc-127">Request body</span></span>
<span data-ttu-id="679dc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="679dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="679dc-129">応答</span><span class="sxs-lookup"><span data-stu-id="679dc-129">Response</span></span>
<span data-ttu-id="679dc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="679dc-130">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679dc-131">例</span><span class="sxs-lookup"><span data-stu-id="679dc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="679dc-132">要求</span><span class="sxs-lookup"><span data-stu-id="679dc-132">Request</span></span>
<span data-ttu-id="679dc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="679dc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="679dc-134">応答</span><span class="sxs-lookup"><span data-stu-id="679dc-134">Response</span></span>
<span data-ttu-id="679dc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="679dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



