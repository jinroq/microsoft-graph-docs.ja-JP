---
title: telecomExpenseManagementPartners のリスト
description: telecomExpenseManagementPartner オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7c9ed2bdfcdaa116d5357fcff07a1ae9e11472e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828085"
---
# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="fc5ab-103">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="fc5ab-103">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="fc5ab-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc5ab-105">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-105">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc5ab-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fc5ab-106">Prerequisites</span></span>
<span data-ttu-id="fc5ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5ab-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc5ab-109">Permission type</span></span>|<span data-ttu-id="fc5ab-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc5ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc5ab-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc5ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc5ab-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc5ab-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc5ab-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc5ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc5ab-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-114">Not supported.</span></span>|
|<span data-ttu-id="fc5ab-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc5ab-115">Application</span></span>|<span data-ttu-id="fc5ab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc5ab-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc5ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="fc5ab-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc5ab-118">Request headers</span></span>
|<span data-ttu-id="fc5ab-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc5ab-119">Header</span></span>|<span data-ttu-id="fc5ab-120">値</span><span class="sxs-lookup"><span data-stu-id="fc5ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc5ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5ab-121">Authorization</span></span>|<span data-ttu-id="fc5ab-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc5ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fc5ab-123">Accept</span></span>|<span data-ttu-id="fc5ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc5ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc5ab-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc5ab-125">Request body</span></span>
<span data-ttu-id="fc5ab-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc5ab-127">応答</span><span class="sxs-lookup"><span data-stu-id="fc5ab-127">Response</span></span>
<span data-ttu-id="fc5ab-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-128">If successful, this method returns a `200 OK` response code and a collection of [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc5ab-129">例</span><span class="sxs-lookup"><span data-stu-id="fc5ab-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc5ab-130">要求</span><span class="sxs-lookup"><span data-stu-id="fc5ab-130">Request</span></span>
<span data-ttu-id="fc5ab-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="fc5ab-132">応答</span><span class="sxs-lookup"><span data-stu-id="fc5ab-132">Response</span></span>
<span data-ttu-id="fc5ab-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fc5ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```



