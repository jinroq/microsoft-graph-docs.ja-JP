---
title: getMobileAppCount 関数
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eab7f9074da1a0aabc33d89108078e6a34a53519
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397779"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="1927e-103">getMobileAppCount 関数</span><span class="sxs-lookup"><span data-stu-id="1927e-103">getMobileAppCount function</span></span>

> <span data-ttu-id="1927e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1927e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1927e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1927e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1927e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1927e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1927e-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1927e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1927e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1927e-108">Prerequisites</span></span>
<span data-ttu-id="1927e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1927e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1927e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1927e-111">Permission type</span></span>|<span data-ttu-id="1927e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1927e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1927e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1927e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1927e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1927e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1927e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1927e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1927e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1927e-116">Not supported.</span></span>|
|<span data-ttu-id="1927e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1927e-117">Application</span></span>|<span data-ttu-id="1927e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1927e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1927e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1927e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="1927e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1927e-120">Request headers</span></span>
|<span data-ttu-id="1927e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1927e-121">Header</span></span>|<span data-ttu-id="1927e-122">値</span><span class="sxs-lookup"><span data-stu-id="1927e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1927e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1927e-123">Authorization</span></span>|<span data-ttu-id="1927e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1927e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1927e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1927e-125">Accept</span></span>|<span data-ttu-id="1927e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1927e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1927e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1927e-127">Request body</span></span>
<span data-ttu-id="1927e-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1927e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1927e-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1927e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1927e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1927e-130">Property</span></span>|<span data-ttu-id="1927e-131">型</span><span class="sxs-lookup"><span data-stu-id="1927e-131">Type</span></span>|<span data-ttu-id="1927e-132">説明</span><span class="sxs-lookup"><span data-stu-id="1927e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1927e-133">status</span><span class="sxs-lookup"><span data-stu-id="1927e-133">status</span></span>|<span data-ttu-id="1927e-134">String</span><span class="sxs-lookup"><span data-stu-id="1927e-134">String</span></span>|<span data-ttu-id="1927e-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1927e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1927e-136">応答</span><span class="sxs-lookup"><span data-stu-id="1927e-136">Response</span></span>
<span data-ttu-id="1927e-137">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に、Int64。</span><span class="sxs-lookup"><span data-stu-id="1927e-137">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1927e-138">例</span><span class="sxs-lookup"><span data-stu-id="1927e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1927e-139">要求</span><span class="sxs-lookup"><span data-stu-id="1927e-139">Request</span></span>
<span data-ttu-id="1927e-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1927e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1927e-141">応答</span><span class="sxs-lookup"><span data-stu-id="1927e-141">Response</span></span>
<span data-ttu-id="1927e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1927e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




