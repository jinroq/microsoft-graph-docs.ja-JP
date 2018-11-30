---
title: getScopesForUser 関数
description: まだ文書化されていません
ms.openlocfilehash: 0cd39dec7cb90623981ee6be1a6c6ad96002d0e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071237"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="7c300-103">getScopesForUser 関数</span><span class="sxs-lookup"><span data-stu-id="7c300-103">getScopesForUser function</span></span>

> <span data-ttu-id="7c300-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c300-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c300-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c300-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c300-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c300-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c300-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7c300-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c300-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c300-108">Prerequisites</span></span>
<span data-ttu-id="7c300-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c300-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c300-111">Permission type</span></span>|<span data-ttu-id="7c300-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c300-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c300-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c300-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c300-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c300-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7c300-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c300-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c300-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c300-116">Not supported.</span></span>|
|<span data-ttu-id="7c300-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c300-117">Application</span></span>|<span data-ttu-id="7c300-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c300-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c300-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c300-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="7c300-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c300-120">Request headers</span></span>
|<span data-ttu-id="7c300-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c300-121">Header</span></span>|<span data-ttu-id="7c300-122">値</span><span class="sxs-lookup"><span data-stu-id="7c300-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c300-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c300-123">Authorization</span></span>|<span data-ttu-id="7c300-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c300-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c300-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c300-125">Accept</span></span>|<span data-ttu-id="7c300-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c300-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c300-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c300-127">Request body</span></span>
<span data-ttu-id="7c300-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c300-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7c300-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7c300-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7c300-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c300-130">Property</span></span>|<span data-ttu-id="7c300-131">型</span><span class="sxs-lookup"><span data-stu-id="7c300-131">Type</span></span>|<span data-ttu-id="7c300-132">説明</span><span class="sxs-lookup"><span data-stu-id="7c300-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c300-133">ユーザー id</span><span class="sxs-lookup"><span data-stu-id="7c300-133">userid</span></span>|<span data-ttu-id="7c300-134">String</span><span class="sxs-lookup"><span data-stu-id="7c300-134">String</span></span>|<span data-ttu-id="7c300-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7c300-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c300-136">応答</span><span class="sxs-lookup"><span data-stu-id="7c300-136">Response</span></span>
<span data-ttu-id="7c300-137">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7c300-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c300-138">例</span><span class="sxs-lookup"><span data-stu-id="7c300-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c300-139">要求</span><span class="sxs-lookup"><span data-stu-id="7c300-139">Request</span></span>
<span data-ttu-id="7c300-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c300-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7c300-141">応答</span><span class="sxs-lookup"><span data-stu-id="7c300-141">Response</span></span>
<span data-ttu-id="7c300-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c300-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





