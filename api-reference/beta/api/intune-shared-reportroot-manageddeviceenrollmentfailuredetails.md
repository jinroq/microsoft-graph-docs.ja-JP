---
title: managedDeviceEnrollmentFailureDetails 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89d5344fce7c4bc0e1545b81ea71c7af632fb442
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350742"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="aea92-103">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="aea92-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="aea92-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="aea92-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aea92-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aea92-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aea92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea92-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aea92-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aea92-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="aea92-108">Prerequisites</span></span>
<span data-ttu-id="aea92-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aea92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aea92-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aea92-111">Permission type</span></span>|<span data-ttu-id="aea92-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aea92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aea92-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aea92-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aea92-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="aea92-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="aea92-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aea92-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aea92-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aea92-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aea92-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea92-117">Not supported.</span></span>|
|<span data-ttu-id="aea92-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aea92-118">Application</span></span>|<span data-ttu-id="aea92-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea92-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aea92-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aea92-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="aea92-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aea92-121">Request headers</span></span>
|<span data-ttu-id="aea92-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aea92-122">Header</span></span>|<span data-ttu-id="aea92-123">値</span><span class="sxs-lookup"><span data-stu-id="aea92-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aea92-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aea92-124">Authorization</span></span>|<span data-ttu-id="aea92-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aea92-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aea92-126">承諾</span><span class="sxs-lookup"><span data-stu-id="aea92-126">Accept</span></span>|<span data-ttu-id="aea92-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aea92-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aea92-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="aea92-128">Request body</span></span>
<span data-ttu-id="aea92-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="aea92-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="aea92-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aea92-130">Property</span></span>|<span data-ttu-id="aea92-131">型</span><span class="sxs-lookup"><span data-stu-id="aea92-131">Type</span></span>|<span data-ttu-id="aea92-132">説明</span><span class="sxs-lookup"><span data-stu-id="aea92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea92-133">フィルター</span><span class="sxs-lookup"><span data-stu-id="aea92-133">filter</span></span>|<span data-ttu-id="aea92-134">String</span><span class="sxs-lookup"><span data-stu-id="aea92-134">String</span></span>|<span data-ttu-id="aea92-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aea92-135">Not yet documented</span></span>|
|<span data-ttu-id="aea92-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="aea92-136">skipToken</span></span>|<span data-ttu-id="aea92-137">String</span><span class="sxs-lookup"><span data-stu-id="aea92-137">String</span></span>|<span data-ttu-id="aea92-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aea92-138">Not yet documented</span></span>|
|<span data-ttu-id="aea92-139">skip</span><span class="sxs-lookup"><span data-stu-id="aea92-139">skip</span></span>|<span data-ttu-id="aea92-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aea92-140">Int32</span></span>|<span data-ttu-id="aea92-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aea92-141">Not yet documented</span></span>|
|<span data-ttu-id="aea92-142">top</span><span class="sxs-lookup"><span data-stu-id="aea92-142">top</span></span>|<span data-ttu-id="aea92-143">Int32</span><span class="sxs-lookup"><span data-stu-id="aea92-143">Int32</span></span>|<span data-ttu-id="aea92-144">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aea92-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aea92-145">応答</span><span class="sxs-lookup"><span data-stu-id="aea92-145">Response</span></span>
<span data-ttu-id="aea92-146">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="aea92-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aea92-147">例</span><span class="sxs-lookup"><span data-stu-id="aea92-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="aea92-148">要求</span><span class="sxs-lookup"><span data-stu-id="aea92-148">Request</span></span>
<span data-ttu-id="aea92-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aea92-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="aea92-150">応答</span><span class="sxs-lookup"><span data-stu-id="aea92-150">Response</span></span>
<span data-ttu-id="aea92-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aea92-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






