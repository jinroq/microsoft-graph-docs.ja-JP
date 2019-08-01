---
title: getAuditActivityTypes 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45ba5a7cf0280e5f54fbbfa00166521ff50e9354
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015906"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="3f2e3-103">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="3f2e3-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="3f2e3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f2e3-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f2e3-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f2e3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f2e3-106">Prerequisites</span></span>
<span data-ttu-id="3f2e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f2e3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f2e3-109">Permission type</span></span>|<span data-ttu-id="3f2e3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f2e3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f2e3-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f2e3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3f2e3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f2e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f2e3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-114">Not supported.</span></span>|
|<span data-ttu-id="3f2e3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f2e3-115">Application</span></span>|<span data-ttu-id="3f2e3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f2e3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f2e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="3f2e3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f2e3-118">Request headers</span></span>
|<span data-ttu-id="3f2e3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f2e3-119">Header</span></span>|<span data-ttu-id="3f2e3-120">値</span><span class="sxs-lookup"><span data-stu-id="3f2e3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f2e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f2e3-121">Authorization</span></span>|<span data-ttu-id="3f2e3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f2e3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="3f2e3-123">Accept</span></span>|<span data-ttu-id="3f2e3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3f2e3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f2e3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f2e3-125">Request body</span></span>
<span data-ttu-id="3f2e3-126">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3f2e3-127">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3f2e3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f2e3-128">Property</span></span>|<span data-ttu-id="3f2e3-129">型</span><span class="sxs-lookup"><span data-stu-id="3f2e3-129">Type</span></span>|<span data-ttu-id="3f2e3-130">説明</span><span class="sxs-lookup"><span data-stu-id="3f2e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f2e3-131">category</span><span class="sxs-lookup"><span data-stu-id="3f2e3-131">category</span></span>|<span data-ttu-id="3f2e3-132">String</span><span class="sxs-lookup"><span data-stu-id="3f2e3-132">String</span></span>|<span data-ttu-id="3f2e3-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f2e3-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f2e3-134">応答</span><span class="sxs-lookup"><span data-stu-id="3f2e3-134">Response</span></span>
<span data-ttu-id="3f2e3-135">成功した場合、この関数は `200 OK` 応答コードと、応答本文で文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f2e3-136">例</span><span class="sxs-lookup"><span data-stu-id="3f2e3-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f2e3-137">要求</span><span class="sxs-lookup"><span data-stu-id="3f2e3-137">Request</span></span>
<span data-ttu-id="3f2e3-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3f2e3-139">応答</span><span class="sxs-lookup"><span data-stu-id="3f2e3-139">Response</span></span>
<span data-ttu-id="3f2e3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f2e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



