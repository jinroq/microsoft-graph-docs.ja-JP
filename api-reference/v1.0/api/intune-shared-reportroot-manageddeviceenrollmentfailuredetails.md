---
title: managedDeviceEnrollmentFailureDetails 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c234181bb70ca0df11cff01b67eb7d6fa60e27ca
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262994"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="13e32-103">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="13e32-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="13e32-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13e32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13e32-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13e32-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13e32-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="13e32-106">Prerequisites</span></span>
<span data-ttu-id="13e32-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13e32-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13e32-109">Permission type</span></span>|<span data-ttu-id="13e32-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13e32-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13e32-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13e32-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="13e32-112">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="13e32-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="13e32-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13e32-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13e32-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13e32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13e32-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13e32-115">Not supported.</span></span>|
|<span data-ttu-id="13e32-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13e32-116">Application</span></span>|<span data-ttu-id="13e32-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13e32-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13e32-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13e32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="13e32-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13e32-119">Request headers</span></span>
|<span data-ttu-id="13e32-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13e32-120">Header</span></span>|<span data-ttu-id="13e32-121">値</span><span class="sxs-lookup"><span data-stu-id="13e32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13e32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13e32-122">Authorization</span></span>|<span data-ttu-id="13e32-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="13e32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13e32-124">承諾</span><span class="sxs-lookup"><span data-stu-id="13e32-124">Accept</span></span>|<span data-ttu-id="13e32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13e32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13e32-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="13e32-126">Request body</span></span>
<span data-ttu-id="13e32-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="13e32-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="13e32-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="13e32-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="13e32-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13e32-129">Property</span></span>|<span data-ttu-id="13e32-130">型</span><span class="sxs-lookup"><span data-stu-id="13e32-130">Type</span></span>|<span data-ttu-id="13e32-131">説明</span><span class="sxs-lookup"><span data-stu-id="13e32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13e32-132">skip</span><span class="sxs-lookup"><span data-stu-id="13e32-132">skip</span></span>|<span data-ttu-id="13e32-133">Int32</span><span class="sxs-lookup"><span data-stu-id="13e32-133">Int32</span></span>|<span data-ttu-id="13e32-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13e32-134">Not yet documented</span></span>|
|<span data-ttu-id="13e32-135">top</span><span class="sxs-lookup"><span data-stu-id="13e32-135">top</span></span>|<span data-ttu-id="13e32-136">Int32</span><span class="sxs-lookup"><span data-stu-id="13e32-136">Int32</span></span>|<span data-ttu-id="13e32-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13e32-137">Not yet documented</span></span>|
|<span data-ttu-id="13e32-138">filter</span><span class="sxs-lookup"><span data-stu-id="13e32-138">filter</span></span>|<span data-ttu-id="13e32-139">String</span><span class="sxs-lookup"><span data-stu-id="13e32-139">String</span></span>|<span data-ttu-id="13e32-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13e32-140">Not yet documented</span></span>|
|<span data-ttu-id="13e32-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="13e32-141">skipToken</span></span>|<span data-ttu-id="13e32-142">String</span><span class="sxs-lookup"><span data-stu-id="13e32-142">String</span></span>|<span data-ttu-id="13e32-143">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="13e32-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13e32-144">応答</span><span class="sxs-lookup"><span data-stu-id="13e32-144">Response</span></span>
<span data-ttu-id="13e32-145">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="13e32-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e32-146">例</span><span class="sxs-lookup"><span data-stu-id="13e32-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="13e32-147">要求</span><span class="sxs-lookup"><span data-stu-id="13e32-147">Request</span></span>
<span data-ttu-id="13e32-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13e32-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="13e32-149">応答</span><span class="sxs-lookup"><span data-stu-id="13e32-149">Response</span></span>
<span data-ttu-id="13e32-150">簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="13e32-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13e32-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="13e32-151">All of the properties will be returned from an actual call.</span></span>

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




