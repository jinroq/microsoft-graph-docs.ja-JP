---
title: managedDeviceEnrollmentAbandonmentDetails 関数
description: 登録 abandonment 詳細レポートのメタデータ
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 618f5985a1d93a9cc45dc4ef93fe475853b7e959
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993551"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="487a8-103">managedDeviceEnrollmentAbandonmentDetails 関数</span><span class="sxs-lookup"><span data-stu-id="487a8-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="487a8-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="487a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="487a8-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="487a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="487a8-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="487a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="487a8-107">登録 abandonment 詳細レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="487a8-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="487a8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="487a8-108">Prerequisites</span></span>
<span data-ttu-id="487a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="487a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="487a8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="487a8-111">Permission type</span></span>|<span data-ttu-id="487a8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="487a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="487a8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="487a8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="487a8-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="487a8-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="487a8-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="487a8-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="487a8-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="487a8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="487a8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="487a8-117">Not supported.</span></span>|
|<span data-ttu-id="487a8-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="487a8-118">Application</span></span>|<span data-ttu-id="487a8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="487a8-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="487a8-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="487a8-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="487a8-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="487a8-121">Request headers</span></span>
|<span data-ttu-id="487a8-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="487a8-122">Header</span></span>|<span data-ttu-id="487a8-123">値</span><span class="sxs-lookup"><span data-stu-id="487a8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="487a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="487a8-124">Authorization</span></span>|<span data-ttu-id="487a8-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="487a8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="487a8-126">承諾</span><span class="sxs-lookup"><span data-stu-id="487a8-126">Accept</span></span>|<span data-ttu-id="487a8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="487a8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="487a8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="487a8-128">Request body</span></span>
<span data-ttu-id="487a8-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="487a8-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="487a8-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="487a8-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="487a8-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="487a8-131">Property</span></span>|<span data-ttu-id="487a8-132">型</span><span class="sxs-lookup"><span data-stu-id="487a8-132">Type</span></span>|<span data-ttu-id="487a8-133">説明</span><span class="sxs-lookup"><span data-stu-id="487a8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="487a8-134">skip</span><span class="sxs-lookup"><span data-stu-id="487a8-134">skip</span></span>|<span data-ttu-id="487a8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="487a8-135">Int32</span></span>|<span data-ttu-id="487a8-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="487a8-136">Not yet documented</span></span>|
|<span data-ttu-id="487a8-137">top</span><span class="sxs-lookup"><span data-stu-id="487a8-137">top</span></span>|<span data-ttu-id="487a8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="487a8-138">Int32</span></span>|<span data-ttu-id="487a8-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="487a8-139">Not yet documented</span></span>|
|<span data-ttu-id="487a8-140">filter</span><span class="sxs-lookup"><span data-stu-id="487a8-140">filter</span></span>|<span data-ttu-id="487a8-141">String</span><span class="sxs-lookup"><span data-stu-id="487a8-141">String</span></span>|<span data-ttu-id="487a8-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="487a8-142">Not yet documented</span></span>|
|<span data-ttu-id="487a8-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="487a8-143">skipToken</span></span>|<span data-ttu-id="487a8-144">String</span><span class="sxs-lookup"><span data-stu-id="487a8-144">String</span></span>|<span data-ttu-id="487a8-145">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="487a8-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="487a8-146">応答</span><span class="sxs-lookup"><span data-stu-id="487a8-146">Response</span></span>
<span data-ttu-id="487a8-147">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="487a8-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="487a8-148">例</span><span class="sxs-lookup"><span data-stu-id="487a8-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="487a8-149">要求</span><span class="sxs-lookup"><span data-stu-id="487a8-149">Request</span></span>
<span data-ttu-id="487a8-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="487a8-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="487a8-151">応答</span><span class="sxs-lookup"><span data-stu-id="487a8-151">Response</span></span>
<span data-ttu-id="487a8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="487a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





