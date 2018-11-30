---
title: managedDeviceEnrollmentFailureDetails 関数
description: まだ文書化されていません
ms.openlocfilehash: c5e68453cb1655e4018156ac207b60e4145e571a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023254"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="6d19b-103">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="6d19b-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="6d19b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d19b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d19b-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6d19b-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d19b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6d19b-106">Prerequisites</span></span>
<span data-ttu-id="6d19b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d19b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d19b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d19b-109">Permission type</span></span>|<span data-ttu-id="6d19b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d19b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d19b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d19b-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6d19b-112">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="6d19b-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6d19b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d19b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6d19b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d19b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d19b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d19b-115">Not supported.</span></span>|
|<span data-ttu-id="6d19b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d19b-116">Application</span></span>|<span data-ttu-id="6d19b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d19b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d19b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d19b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="6d19b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d19b-119">Request headers</span></span>
|<span data-ttu-id="6d19b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d19b-120">Header</span></span>|<span data-ttu-id="6d19b-121">値</span><span class="sxs-lookup"><span data-stu-id="6d19b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d19b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d19b-122">Authorization</span></span>|<span data-ttu-id="6d19b-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6d19b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d19b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6d19b-124">Accept</span></span>|<span data-ttu-id="6d19b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d19b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d19b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d19b-126">Request body</span></span>
<span data-ttu-id="6d19b-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d19b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6d19b-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="6d19b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6d19b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d19b-129">Property</span></span>|<span data-ttu-id="6d19b-130">型</span><span class="sxs-lookup"><span data-stu-id="6d19b-130">Type</span></span>|<span data-ttu-id="6d19b-131">説明</span><span class="sxs-lookup"><span data-stu-id="6d19b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d19b-132">skip</span><span class="sxs-lookup"><span data-stu-id="6d19b-132">skip</span></span>|<span data-ttu-id="6d19b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6d19b-133">Int32</span></span>|<span data-ttu-id="6d19b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6d19b-134">Not yet documented</span></span>|
|<span data-ttu-id="6d19b-135">top</span><span class="sxs-lookup"><span data-stu-id="6d19b-135">top</span></span>|<span data-ttu-id="6d19b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6d19b-136">Int32</span></span>|<span data-ttu-id="6d19b-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6d19b-137">Not yet documented</span></span>|
|<span data-ttu-id="6d19b-138">filter</span><span class="sxs-lookup"><span data-stu-id="6d19b-138">filter</span></span>|<span data-ttu-id="6d19b-139">String</span><span class="sxs-lookup"><span data-stu-id="6d19b-139">String</span></span>|<span data-ttu-id="6d19b-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6d19b-140">Not yet documented</span></span>|
|<span data-ttu-id="6d19b-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="6d19b-141">skipToken</span></span>|<span data-ttu-id="6d19b-142">String</span><span class="sxs-lookup"><span data-stu-id="6d19b-142">String</span></span>|<span data-ttu-id="6d19b-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6d19b-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d19b-144">応答</span><span class="sxs-lookup"><span data-stu-id="6d19b-144">Response</span></span>
<span data-ttu-id="6d19b-145">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="6d19b-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d19b-146">例</span><span class="sxs-lookup"><span data-stu-id="6d19b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d19b-147">要求</span><span class="sxs-lookup"><span data-stu-id="6d19b-147">Request</span></span>
<span data-ttu-id="6d19b-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d19b-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6d19b-149">応答</span><span class="sxs-lookup"><span data-stu-id="6d19b-149">Response</span></span>
<span data-ttu-id="6d19b-150">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="6d19b-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6d19b-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d19b-151">All of the properties will be returned from an actual call.</span></span>

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




