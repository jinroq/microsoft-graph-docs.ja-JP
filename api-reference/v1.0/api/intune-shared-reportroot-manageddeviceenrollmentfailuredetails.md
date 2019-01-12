---
title: managedDeviceEnrollmentFailureDetails 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 128ad6e3985649b3dbaffa101c19f0b2440b0838
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980378"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="29eed-103">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="29eed-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="29eed-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29eed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29eed-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29eed-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29eed-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="29eed-106">Prerequisites</span></span>
<span data-ttu-id="29eed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29eed-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29eed-109">Permission type</span></span>|<span data-ttu-id="29eed-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29eed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29eed-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29eed-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="29eed-112">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="29eed-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="29eed-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29eed-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29eed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29eed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29eed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29eed-115">Not supported.</span></span>|
|<span data-ttu-id="29eed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29eed-116">Application</span></span>|<span data-ttu-id="29eed-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29eed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29eed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29eed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="29eed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29eed-119">Request headers</span></span>
|<span data-ttu-id="29eed-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29eed-120">Header</span></span>|<span data-ttu-id="29eed-121">値</span><span class="sxs-lookup"><span data-stu-id="29eed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29eed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29eed-122">Authorization</span></span>|<span data-ttu-id="29eed-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="29eed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29eed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="29eed-124">Accept</span></span>|<span data-ttu-id="29eed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29eed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29eed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="29eed-126">Request body</span></span>
<span data-ttu-id="29eed-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="29eed-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="29eed-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="29eed-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="29eed-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29eed-129">Property</span></span>|<span data-ttu-id="29eed-130">型</span><span class="sxs-lookup"><span data-stu-id="29eed-130">Type</span></span>|<span data-ttu-id="29eed-131">説明</span><span class="sxs-lookup"><span data-stu-id="29eed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29eed-132">skip</span><span class="sxs-lookup"><span data-stu-id="29eed-132">skip</span></span>|<span data-ttu-id="29eed-133">Int32</span><span class="sxs-lookup"><span data-stu-id="29eed-133">Int32</span></span>|<span data-ttu-id="29eed-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29eed-134">Not yet documented</span></span>|
|<span data-ttu-id="29eed-135">top</span><span class="sxs-lookup"><span data-stu-id="29eed-135">top</span></span>|<span data-ttu-id="29eed-136">Int32</span><span class="sxs-lookup"><span data-stu-id="29eed-136">Int32</span></span>|<span data-ttu-id="29eed-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29eed-137">Not yet documented</span></span>|
|<span data-ttu-id="29eed-138">filter</span><span class="sxs-lookup"><span data-stu-id="29eed-138">filter</span></span>|<span data-ttu-id="29eed-139">String</span><span class="sxs-lookup"><span data-stu-id="29eed-139">String</span></span>|<span data-ttu-id="29eed-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29eed-140">Not yet documented</span></span>|
|<span data-ttu-id="29eed-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="29eed-141">skipToken</span></span>|<span data-ttu-id="29eed-142">String</span><span class="sxs-lookup"><span data-stu-id="29eed-142">String</span></span>|<span data-ttu-id="29eed-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="29eed-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29eed-144">応答</span><span class="sxs-lookup"><span data-stu-id="29eed-144">Response</span></span>
<span data-ttu-id="29eed-145">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="29eed-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29eed-146">例</span><span class="sxs-lookup"><span data-stu-id="29eed-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="29eed-147">要求</span><span class="sxs-lookup"><span data-stu-id="29eed-147">Request</span></span>
<span data-ttu-id="29eed-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29eed-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="29eed-149">応答</span><span class="sxs-lookup"><span data-stu-id="29eed-149">Response</span></span>
<span data-ttu-id="29eed-150">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="29eed-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="29eed-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="29eed-151">All of the properties will be returned from an actual call.</span></span>

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




