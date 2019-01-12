---
title: managedDeviceEnrollmentFailureTrends 関数
description: 登録の失敗の傾向レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 648053ad000b2a9988b46b0d68d62219ed967a3a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963634"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="b040f-103">managedDeviceEnrollmentFailureTrends 関数</span><span class="sxs-lookup"><span data-stu-id="b040f-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="b040f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b040f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b040f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b040f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b040f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b040f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b040f-107">登録の失敗の傾向レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="b040f-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b040f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b040f-108">Prerequisites</span></span>
<span data-ttu-id="b040f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b040f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b040f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b040f-111">Permission type</span></span>|<span data-ttu-id="b040f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b040f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b040f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b040f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b040f-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b040f-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b040f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b040f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b040f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b040f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b040f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b040f-117">Not supported.</span></span>|
|<span data-ttu-id="b040f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b040f-118">Application</span></span>|<span data-ttu-id="b040f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b040f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b040f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b040f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="b040f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b040f-121">Request headers</span></span>
|<span data-ttu-id="b040f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b040f-122">Header</span></span>|<span data-ttu-id="b040f-123">値</span><span class="sxs-lookup"><span data-stu-id="b040f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b040f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b040f-124">Authorization</span></span>|<span data-ttu-id="b040f-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b040f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b040f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b040f-126">Accept</span></span>|<span data-ttu-id="b040f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b040f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b040f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b040f-128">Request body</span></span>
<span data-ttu-id="b040f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b040f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b040f-130">応答</span><span class="sxs-lookup"><span data-stu-id="b040f-130">Response</span></span>
<span data-ttu-id="b040f-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="b040f-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b040f-132">例</span><span class="sxs-lookup"><span data-stu-id="b040f-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="b040f-133">要求</span><span class="sxs-lookup"><span data-stu-id="b040f-133">Request</span></span>
<span data-ttu-id="b040f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b040f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="b040f-135">応答</span><span class="sxs-lookup"><span data-stu-id="b040f-135">Response</span></span>
<span data-ttu-id="b040f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b040f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



