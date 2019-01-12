---
title: managedDeviceEnrollmentFailureDetails 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 48f7f2c36781be29842c1c614e8d2a14ec7e1d94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915117"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="b3844-103">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="b3844-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="b3844-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3844-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3844-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3844-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3844-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3844-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3844-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3844-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3844-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3844-108">Prerequisites</span></span>
<span data-ttu-id="b3844-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3844-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3844-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3844-111">Permission type</span></span>|<span data-ttu-id="b3844-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3844-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3844-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3844-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b3844-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b3844-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b3844-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3844-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b3844-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3844-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3844-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3844-117">Not supported.</span></span>|
|<span data-ttu-id="b3844-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3844-118">Application</span></span>|<span data-ttu-id="b3844-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3844-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3844-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3844-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="b3844-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3844-121">Request headers</span></span>
|<span data-ttu-id="b3844-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3844-122">Header</span></span>|<span data-ttu-id="b3844-123">値</span><span class="sxs-lookup"><span data-stu-id="b3844-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3844-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3844-124">Authorization</span></span>|<span data-ttu-id="b3844-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3844-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3844-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b3844-126">Accept</span></span>|<span data-ttu-id="b3844-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b3844-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3844-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3844-128">Request body</span></span>
<span data-ttu-id="b3844-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="b3844-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b3844-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3844-130">Property</span></span>|<span data-ttu-id="b3844-131">種類</span><span class="sxs-lookup"><span data-stu-id="b3844-131">Type</span></span>|<span data-ttu-id="b3844-132">説明</span><span class="sxs-lookup"><span data-stu-id="b3844-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3844-133">filter</span><span class="sxs-lookup"><span data-stu-id="b3844-133">filter</span></span>|<span data-ttu-id="b3844-134">String</span><span class="sxs-lookup"><span data-stu-id="b3844-134">String</span></span>|<span data-ttu-id="b3844-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3844-135">Not yet documented</span></span>|
|<span data-ttu-id="b3844-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="b3844-136">skipToken</span></span>|<span data-ttu-id="b3844-137">String</span><span class="sxs-lookup"><span data-stu-id="b3844-137">String</span></span>|<span data-ttu-id="b3844-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3844-138">Not yet documented</span></span>|
|<span data-ttu-id="b3844-139">skip</span><span class="sxs-lookup"><span data-stu-id="b3844-139">skip</span></span>|<span data-ttu-id="b3844-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b3844-140">Int32</span></span>|<span data-ttu-id="b3844-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3844-141">Not yet documented</span></span>|
|<span data-ttu-id="b3844-142">top</span><span class="sxs-lookup"><span data-stu-id="b3844-142">top</span></span>|<span data-ttu-id="b3844-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b3844-143">Int32</span></span>|<span data-ttu-id="b3844-144">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3844-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3844-145">応答</span><span class="sxs-lookup"><span data-stu-id="b3844-145">Response</span></span>
<span data-ttu-id="b3844-146">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="b3844-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3844-147">例</span><span class="sxs-lookup"><span data-stu-id="b3844-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3844-148">要求</span><span class="sxs-lookup"><span data-stu-id="b3844-148">Request</span></span>
<span data-ttu-id="b3844-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3844-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b3844-150">応答</span><span class="sxs-lookup"><span data-stu-id="b3844-150">Response</span></span>
<span data-ttu-id="b3844-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3844-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



