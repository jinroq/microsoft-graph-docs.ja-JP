---
title: managedDeviceEnrollmentTopFailures 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4a21d9fc0b29c63053d184db235a1c44744d8e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932659"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="3c80f-103">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="3c80f-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="3c80f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c80f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c80f-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c80f-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c80f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3c80f-106">Prerequisites</span></span>
<span data-ttu-id="3c80f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c80f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c80f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c80f-109">Permission type</span></span>|<span data-ttu-id="3c80f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c80f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c80f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c80f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c80f-112">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="3c80f-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3c80f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c80f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3c80f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c80f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c80f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c80f-115">Not supported.</span></span>|
|<span data-ttu-id="3c80f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c80f-116">Application</span></span>|<span data-ttu-id="3c80f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c80f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c80f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c80f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="3c80f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c80f-119">Request headers</span></span>
|<span data-ttu-id="3c80f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c80f-120">Header</span></span>|<span data-ttu-id="3c80f-121">値</span><span class="sxs-lookup"><span data-stu-id="3c80f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c80f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c80f-122">Authorization</span></span>|<span data-ttu-id="3c80f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3c80f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c80f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3c80f-124">Accept</span></span>|<span data-ttu-id="3c80f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c80f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c80f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c80f-126">Request body</span></span>
<span data-ttu-id="3c80f-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c80f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3c80f-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3c80f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3c80f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c80f-129">Property</span></span>|<span data-ttu-id="3c80f-130">種類</span><span class="sxs-lookup"><span data-stu-id="3c80f-130">Type</span></span>|<span data-ttu-id="3c80f-131">説明</span><span class="sxs-lookup"><span data-stu-id="3c80f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c80f-132">period</span><span class="sxs-lookup"><span data-stu-id="3c80f-132">period</span></span>|<span data-ttu-id="3c80f-133">String</span><span class="sxs-lookup"><span data-stu-id="3c80f-133">String</span></span>|<span data-ttu-id="3c80f-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3c80f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3c80f-135">応答</span><span class="sxs-lookup"><span data-stu-id="3c80f-135">Response</span></span>
<span data-ttu-id="3c80f-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="3c80f-136">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c80f-137">例</span><span class="sxs-lookup"><span data-stu-id="3c80f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c80f-138">要求</span><span class="sxs-lookup"><span data-stu-id="3c80f-138">Request</span></span>
<span data-ttu-id="3c80f-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c80f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3c80f-140">応答</span><span class="sxs-lookup"><span data-stu-id="3c80f-140">Response</span></span>
<span data-ttu-id="3c80f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c80f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




