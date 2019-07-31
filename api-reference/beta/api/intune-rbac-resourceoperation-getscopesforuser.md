---
title: getScopesForUser 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e57387ba4ff5e5af3c3d1a599ee33c7f2a3e1b99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980045"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="cbb99-103">getScopesForUser 関数</span><span class="sxs-lookup"><span data-stu-id="cbb99-103">getScopesForUser function</span></span>

> <span data-ttu-id="cbb99-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbb99-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbb99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbb99-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cbb99-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbb99-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cbb99-107">Prerequisites</span></span>
<span data-ttu-id="cbb99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbb99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbb99-110">Permission type</span></span>|<span data-ttu-id="cbb99-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbb99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbb99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbb99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbb99-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbb99-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="cbb99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbb99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbb99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb99-115">Not supported.</span></span>|
|<span data-ttu-id="cbb99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbb99-116">Application</span></span>|<span data-ttu-id="cbb99-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbb99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbb99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="cbb99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbb99-119">Request headers</span></span>
|<span data-ttu-id="cbb99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbb99-120">Header</span></span>|<span data-ttu-id="cbb99-121">値</span><span class="sxs-lookup"><span data-stu-id="cbb99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbb99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbb99-122">Authorization</span></span>|<span data-ttu-id="cbb99-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cbb99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbb99-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cbb99-124">Accept</span></span>|<span data-ttu-id="cbb99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbb99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbb99-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbb99-126">Request body</span></span>
<span data-ttu-id="cbb99-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="cbb99-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cbb99-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="cbb99-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cbb99-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbb99-129">Property</span></span>|<span data-ttu-id="cbb99-130">型</span><span class="sxs-lookup"><span data-stu-id="cbb99-130">Type</span></span>|<span data-ttu-id="cbb99-131">説明</span><span class="sxs-lookup"><span data-stu-id="cbb99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbb99-132">userid</span><span class="sxs-lookup"><span data-stu-id="cbb99-132">userid</span></span>|<span data-ttu-id="cbb99-133">String</span><span class="sxs-lookup"><span data-stu-id="cbb99-133">String</span></span>|<span data-ttu-id="cbb99-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cbb99-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbb99-135">応答</span><span class="sxs-lookup"><span data-stu-id="cbb99-135">Response</span></span>
<span data-ttu-id="cbb99-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cbb99-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbb99-137">例</span><span class="sxs-lookup"><span data-stu-id="cbb99-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbb99-138">要求</span><span class="sxs-lookup"><span data-stu-id="cbb99-138">Request</span></span>
<span data-ttu-id="cbb99-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbb99-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cbb99-140">応答</span><span class="sxs-lookup"><span data-stu-id="cbb99-140">Response</span></span>
<span data-ttu-id="cbb99-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cbb99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```





