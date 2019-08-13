---
title: getAuditActivityTypes 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7378b2e77ba15dc2117ae18b70c1adbf5652c24
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328591"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="5ad0c-103">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="5ad0c-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="5ad0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ad0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ad0c-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5ad0c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ad0c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5ad0c-107">Prerequisites</span></span>
<span data-ttu-id="5ad0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ad0c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ad0c-110">Permission type</span></span>|<span data-ttu-id="5ad0c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ad0c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ad0c-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ad0c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5ad0c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ad0c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-115">Not supported.</span></span>|
|<span data-ttu-id="5ad0c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ad0c-116">Application</span></span>|<span data-ttu-id="5ad0c-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ad0c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ad0c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ad0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="5ad0c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ad0c-119">Request headers</span></span>
|<span data-ttu-id="5ad0c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ad0c-120">Header</span></span>|<span data-ttu-id="5ad0c-121">値</span><span class="sxs-lookup"><span data-stu-id="5ad0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ad0c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ad0c-122">Authorization</span></span>|<span data-ttu-id="5ad0c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ad0c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5ad0c-124">Accept</span></span>|<span data-ttu-id="5ad0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ad0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ad0c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ad0c-126">Request body</span></span>
<span data-ttu-id="5ad0c-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5ad0c-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5ad0c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ad0c-129">Property</span></span>|<span data-ttu-id="5ad0c-130">型</span><span class="sxs-lookup"><span data-stu-id="5ad0c-130">Type</span></span>|<span data-ttu-id="5ad0c-131">説明</span><span class="sxs-lookup"><span data-stu-id="5ad0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad0c-132">category</span><span class="sxs-lookup"><span data-stu-id="5ad0c-132">category</span></span>|<span data-ttu-id="5ad0c-133">String</span><span class="sxs-lookup"><span data-stu-id="5ad0c-133">String</span></span>|<span data-ttu-id="5ad0c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5ad0c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5ad0c-135">応答</span><span class="sxs-lookup"><span data-stu-id="5ad0c-135">Response</span></span>
<span data-ttu-id="5ad0c-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ad0c-137">例</span><span class="sxs-lookup"><span data-stu-id="5ad0c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ad0c-138">要求</span><span class="sxs-lookup"><span data-stu-id="5ad0c-138">Request</span></span>
<span data-ttu-id="5ad0c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5ad0c-140">応答</span><span class="sxs-lookup"><span data-stu-id="5ad0c-140">Response</span></span>
<span data-ttu-id="5ad0c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ad0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






