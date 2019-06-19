---
title: scopedForResource 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0745ef277ad852ef061ea0f4f352cf07e808604
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002267"
---
# <a name="scopedforresource-function"></a><span data-ttu-id="585e6-103">scopedForResource 関数</span><span class="sxs-lookup"><span data-stu-id="585e6-103">scopedForResource function</span></span>

> <span data-ttu-id="585e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="585e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="585e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="585e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="585e6-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="585e6-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="585e6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="585e6-107">Prerequisites</span></span>
<span data-ttu-id="585e6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="585e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="585e6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="585e6-110">Permission type</span></span>|<span data-ttu-id="585e6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="585e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="585e6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="585e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="585e6-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="585e6-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="585e6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="585e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="585e6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="585e6-115">Not supported.</span></span>|
|<span data-ttu-id="585e6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="585e6-116">Application</span></span>|<span data-ttu-id="585e6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="585e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="585e6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="585e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/scopedForResource
```

## <a name="request-headers"></a><span data-ttu-id="585e6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="585e6-119">Request headers</span></span>
|<span data-ttu-id="585e6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="585e6-120">Header</span></span>|<span data-ttu-id="585e6-121">値</span><span class="sxs-lookup"><span data-stu-id="585e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="585e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="585e6-122">Authorization</span></span>|<span data-ttu-id="585e6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="585e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="585e6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="585e6-124">Accept</span></span>|<span data-ttu-id="585e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="585e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="585e6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="585e6-126">Request body</span></span>
<span data-ttu-id="585e6-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="585e6-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="585e6-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="585e6-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="585e6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="585e6-129">Property</span></span>|<span data-ttu-id="585e6-130">型</span><span class="sxs-lookup"><span data-stu-id="585e6-130">Type</span></span>|<span data-ttu-id="585e6-131">説明</span><span class="sxs-lookup"><span data-stu-id="585e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="585e6-132">リソース</span><span class="sxs-lookup"><span data-stu-id="585e6-132">resource</span></span>|<span data-ttu-id="585e6-133">String</span><span class="sxs-lookup"><span data-stu-id="585e6-133">String</span></span>|<span data-ttu-id="585e6-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="585e6-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="585e6-135">応答</span><span class="sxs-lookup"><span data-stu-id="585e6-135">Response</span></span>
<span data-ttu-id="585e6-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文でブール値を返します。</span><span class="sxs-lookup"><span data-stu-id="585e6-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="585e6-137">例</span><span class="sxs-lookup"><span data-stu-id="585e6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="585e6-138">要求</span><span class="sxs-lookup"><span data-stu-id="585e6-138">Request</span></span>
<span data-ttu-id="585e6-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="585e6-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/scopedForResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="585e6-140">応答</span><span class="sxs-lookup"><span data-stu-id="585e6-140">Response</span></span>
<span data-ttu-id="585e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="585e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




