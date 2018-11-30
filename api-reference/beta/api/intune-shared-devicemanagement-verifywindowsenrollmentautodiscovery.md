---
title: verifyWindowsEnrollmentAutoDiscovery 関数
description: まだ文書化されていません
ms.openlocfilehash: ecccb32089a2547d4b130943e9afc8c6d7caebf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072142"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="3639d-103">verifyWindowsEnrollmentAutoDiscovery 関数</span><span class="sxs-lookup"><span data-stu-id="3639d-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="3639d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3639d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3639d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3639d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3639d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3639d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3639d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3639d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3639d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3639d-108">Prerequisites</span></span>
<span data-ttu-id="3639d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3639d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3639d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3639d-111">Permission type</span></span>|<span data-ttu-id="3639d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3639d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3639d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3639d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3639d-114">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="3639d-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3639d-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3639d-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3639d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3639d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3639d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3639d-117">Not supported.</span></span>|
|<span data-ttu-id="3639d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3639d-118">Application</span></span>|<span data-ttu-id="3639d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3639d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3639d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3639d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="3639d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3639d-121">Request headers</span></span>
|<span data-ttu-id="3639d-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3639d-122">Header</span></span>|<span data-ttu-id="3639d-123">値</span><span class="sxs-lookup"><span data-stu-id="3639d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3639d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3639d-124">Authorization</span></span>|<span data-ttu-id="3639d-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3639d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3639d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3639d-126">Accept</span></span>|<span data-ttu-id="3639d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3639d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3639d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3639d-128">Request body</span></span>
<span data-ttu-id="3639d-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3639d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3639d-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3639d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3639d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3639d-131">Property</span></span>|<span data-ttu-id="3639d-132">型</span><span class="sxs-lookup"><span data-stu-id="3639d-132">Type</span></span>|<span data-ttu-id="3639d-133">説明</span><span class="sxs-lookup"><span data-stu-id="3639d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3639d-134">domainName</span><span class="sxs-lookup"><span data-stu-id="3639d-134">domainName</span></span>|<span data-ttu-id="3639d-135">String</span><span class="sxs-lookup"><span data-stu-id="3639d-135">String</span></span>|<span data-ttu-id="3639d-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3639d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3639d-137">応答</span><span class="sxs-lookup"><span data-stu-id="3639d-137">Response</span></span>
<span data-ttu-id="3639d-138">成功した場合、この関数は `200 OK` 応答コードと、応答本文でブール値を返します。</span><span class="sxs-lookup"><span data-stu-id="3639d-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3639d-139">例</span><span class="sxs-lookup"><span data-stu-id="3639d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3639d-140">要求</span><span class="sxs-lookup"><span data-stu-id="3639d-140">Request</span></span>
<span data-ttu-id="3639d-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3639d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3639d-142">応答</span><span class="sxs-lookup"><span data-stu-id="3639d-142">Response</span></span>
<span data-ttu-id="3639d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3639d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



