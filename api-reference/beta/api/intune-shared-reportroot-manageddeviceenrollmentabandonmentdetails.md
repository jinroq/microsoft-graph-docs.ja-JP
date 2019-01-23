---
title: managedDeviceEnrollmentAbandonmentDetails 関数
description: 登録放棄の詳細レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 30312706926293e24226801a7e0193b28d3d6f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393215"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="b6f59-103">managedDeviceEnrollmentAbandonmentDetails 関数</span><span class="sxs-lookup"><span data-stu-id="b6f59-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="b6f59-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b6f59-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6f59-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6f59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6f59-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6f59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f59-107">登録放棄の詳細レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="b6f59-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6f59-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6f59-108">Prerequisites</span></span>
<span data-ttu-id="b6f59-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6f59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f59-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6f59-111">Permission type</span></span>|<span data-ttu-id="b6f59-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6f59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f59-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6f59-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6f59-114">&nbsp;&nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b6f59-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="b6f59-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f59-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b6f59-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6f59-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f59-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6f59-117">Not supported.</span></span>|
|<span data-ttu-id="b6f59-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6f59-118">Application</span></span>|<span data-ttu-id="b6f59-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6f59-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f59-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6f59-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="b6f59-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6f59-121">Request headers</span></span>
|<span data-ttu-id="b6f59-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6f59-122">Header</span></span>|<span data-ttu-id="b6f59-123">値</span><span class="sxs-lookup"><span data-stu-id="b6f59-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f59-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f59-124">Authorization</span></span>|<span data-ttu-id="b6f59-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b6f59-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f59-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b6f59-126">Accept</span></span>|<span data-ttu-id="b6f59-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f59-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f59-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6f59-128">Request body</span></span>
<span data-ttu-id="b6f59-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6f59-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b6f59-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="b6f59-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b6f59-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6f59-131">Property</span></span>|<span data-ttu-id="b6f59-132">型</span><span class="sxs-lookup"><span data-stu-id="b6f59-132">Type</span></span>|<span data-ttu-id="b6f59-133">説明</span><span class="sxs-lookup"><span data-stu-id="b6f59-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f59-134">skip</span><span class="sxs-lookup"><span data-stu-id="b6f59-134">skip</span></span>|<span data-ttu-id="b6f59-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b6f59-135">Int32</span></span>|<span data-ttu-id="b6f59-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b6f59-136">Not yet documented</span></span>|
|<span data-ttu-id="b6f59-137">top</span><span class="sxs-lookup"><span data-stu-id="b6f59-137">top</span></span>|<span data-ttu-id="b6f59-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b6f59-138">Int32</span></span>|<span data-ttu-id="b6f59-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b6f59-139">Not yet documented</span></span>|
|<span data-ttu-id="b6f59-140">filter</span><span class="sxs-lookup"><span data-stu-id="b6f59-140">filter</span></span>|<span data-ttu-id="b6f59-141">String</span><span class="sxs-lookup"><span data-stu-id="b6f59-141">String</span></span>|<span data-ttu-id="b6f59-142">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b6f59-142">Not yet documented</span></span>|
|<span data-ttu-id="b6f59-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="b6f59-143">skipToken</span></span>|<span data-ttu-id="b6f59-144">String</span><span class="sxs-lookup"><span data-stu-id="b6f59-144">String</span></span>|<span data-ttu-id="b6f59-145">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b6f59-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6f59-146">応答</span><span class="sxs-lookup"><span data-stu-id="b6f59-146">Response</span></span>
<span data-ttu-id="b6f59-147">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="b6f59-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f59-148">例</span><span class="sxs-lookup"><span data-stu-id="b6f59-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6f59-149">要求</span><span class="sxs-lookup"><span data-stu-id="b6f59-149">Request</span></span>
<span data-ttu-id="b6f59-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6f59-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b6f59-151">応答</span><span class="sxs-lookup"><span data-stu-id="b6f59-151">Response</span></span>
<span data-ttu-id="b6f59-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6f59-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





