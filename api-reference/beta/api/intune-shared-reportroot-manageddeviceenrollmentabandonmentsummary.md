---
title: managedDeviceEnrollmentAbandonmentSummary 関数
description: 登録 abandonment の概要レポートのメタデータ
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d988136da29680bd32b2ff24427bbf69135ab10
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350777"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="7cf1a-103">managedDeviceEnrollmentAbandonmentSummary 関数</span><span class="sxs-lookup"><span data-stu-id="7cf1a-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="7cf1a-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7cf1a-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cf1a-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cf1a-107">登録 abandonment の概要レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="7cf1a-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cf1a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cf1a-108">Prerequisites</span></span>
<span data-ttu-id="7cf1a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf1a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cf1a-111">Permission type</span></span>|<span data-ttu-id="7cf1a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cf1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cf1a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cf1a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7cf1a-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="7cf1a-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="7cf1a-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf1a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7cf1a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cf1a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cf1a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-117">Not supported.</span></span>|
|<span data-ttu-id="7cf1a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cf1a-118">Application</span></span>|<span data-ttu-id="7cf1a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cf1a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cf1a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="7cf1a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cf1a-121">Request headers</span></span>
|<span data-ttu-id="7cf1a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cf1a-122">Header</span></span>|<span data-ttu-id="7cf1a-123">値</span><span class="sxs-lookup"><span data-stu-id="7cf1a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cf1a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cf1a-124">Authorization</span></span>|<span data-ttu-id="7cf1a-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cf1a-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7cf1a-126">Accept</span></span>|<span data-ttu-id="7cf1a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7cf1a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cf1a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cf1a-128">Request body</span></span>
<span data-ttu-id="7cf1a-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7cf1a-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7cf1a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cf1a-131">Property</span></span>|<span data-ttu-id="7cf1a-132">型</span><span class="sxs-lookup"><span data-stu-id="7cf1a-132">Type</span></span>|<span data-ttu-id="7cf1a-133">説明</span><span class="sxs-lookup"><span data-stu-id="7cf1a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cf1a-134">skip</span><span class="sxs-lookup"><span data-stu-id="7cf1a-134">skip</span></span>|<span data-ttu-id="7cf1a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7cf1a-135">Int32</span></span>|<span data-ttu-id="7cf1a-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7cf1a-136">Not yet documented</span></span>|
|<span data-ttu-id="7cf1a-137">top</span><span class="sxs-lookup"><span data-stu-id="7cf1a-137">top</span></span>|<span data-ttu-id="7cf1a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7cf1a-138">Int32</span></span>|<span data-ttu-id="7cf1a-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7cf1a-139">Not yet documented</span></span>|
|<span data-ttu-id="7cf1a-140">filter</span><span class="sxs-lookup"><span data-stu-id="7cf1a-140">filter</span></span>|<span data-ttu-id="7cf1a-141">String</span><span class="sxs-lookup"><span data-stu-id="7cf1a-141">String</span></span>|<span data-ttu-id="7cf1a-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7cf1a-142">Not yet documented</span></span>|
|<span data-ttu-id="7cf1a-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="7cf1a-143">skipToken</span></span>|<span data-ttu-id="7cf1a-144">String</span><span class="sxs-lookup"><span data-stu-id="7cf1a-144">String</span></span>|<span data-ttu-id="7cf1a-145">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7cf1a-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7cf1a-146">応答</span><span class="sxs-lookup"><span data-stu-id="7cf1a-146">Response</span></span>
<span data-ttu-id="7cf1a-147">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cf1a-148">例</span><span class="sxs-lookup"><span data-stu-id="7cf1a-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cf1a-149">要求</span><span class="sxs-lookup"><span data-stu-id="7cf1a-149">Request</span></span>
<span data-ttu-id="7cf1a-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7cf1a-151">応答</span><span class="sxs-lookup"><span data-stu-id="7cf1a-151">Response</span></span>
<span data-ttu-id="7cf1a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cf1a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








