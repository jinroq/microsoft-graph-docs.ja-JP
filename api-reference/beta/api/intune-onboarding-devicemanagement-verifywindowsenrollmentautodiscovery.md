---
title: verifyWindowsEnrollmentAutoDiscovery 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c0afcb22adddb64863f45e0a07f45f3f5d10513
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984533"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="2253b-103">verifyWindowsEnrollmentAutoDiscovery 関数</span><span class="sxs-lookup"><span data-stu-id="2253b-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="2253b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2253b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2253b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2253b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2253b-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2253b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2253b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2253b-107">Prerequisites</span></span>
<span data-ttu-id="2253b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2253b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2253b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2253b-110">Permission type</span></span>|<span data-ttu-id="2253b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2253b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2253b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2253b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2253b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2253b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2253b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2253b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2253b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2253b-115">Not supported.</span></span>|
|<span data-ttu-id="2253b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2253b-116">Application</span></span>|<span data-ttu-id="2253b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2253b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2253b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2253b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="2253b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2253b-119">Request headers</span></span>
|<span data-ttu-id="2253b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2253b-120">Header</span></span>|<span data-ttu-id="2253b-121">値</span><span class="sxs-lookup"><span data-stu-id="2253b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2253b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2253b-122">Authorization</span></span>|<span data-ttu-id="2253b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2253b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2253b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2253b-124">Accept</span></span>|<span data-ttu-id="2253b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2253b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2253b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2253b-126">Request body</span></span>
<span data-ttu-id="2253b-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2253b-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2253b-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="2253b-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2253b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2253b-129">Property</span></span>|<span data-ttu-id="2253b-130">型</span><span class="sxs-lookup"><span data-stu-id="2253b-130">Type</span></span>|<span data-ttu-id="2253b-131">説明</span><span class="sxs-lookup"><span data-stu-id="2253b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2253b-132">domainName</span><span class="sxs-lookup"><span data-stu-id="2253b-132">domainName</span></span>|<span data-ttu-id="2253b-133">String</span><span class="sxs-lookup"><span data-stu-id="2253b-133">String</span></span>|<span data-ttu-id="2253b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2253b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2253b-135">応答</span><span class="sxs-lookup"><span data-stu-id="2253b-135">Response</span></span>
<span data-ttu-id="2253b-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文でブール値を返します。</span><span class="sxs-lookup"><span data-stu-id="2253b-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2253b-137">例</span><span class="sxs-lookup"><span data-stu-id="2253b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="2253b-138">要求</span><span class="sxs-lookup"><span data-stu-id="2253b-138">Request</span></span>
<span data-ttu-id="2253b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2253b-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2253b-140">応答</span><span class="sxs-lookup"><span data-stu-id="2253b-140">Response</span></span>
<span data-ttu-id="2253b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2253b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





