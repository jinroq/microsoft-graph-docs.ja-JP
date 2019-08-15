---
title: Get plannerPlan
description: '**plannerplan** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c1adf51f5dec48a9eb198904c2e38ca07f08537c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413323"
---
# <a name="get-plannerplan"></a><span data-ttu-id="60b2d-103">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="60b2d-103">Get plannerPlan</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b2d-104">[Plan](../resources/plannerplan.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="60b2d-104">Retrieve the properties and relationships of a [plannerplan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60b2d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60b2d-105">Permissions</span></span>
<span data-ttu-id="60b2d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60b2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b2d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60b2d-108">Permission type</span></span>      | <span data-ttu-id="60b2d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60b2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b2d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60b2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60b2d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b2d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60b2d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60b2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60b2d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60b2d-113">Not supported.</span></span>    |
|<span data-ttu-id="60b2d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60b2d-114">Application</span></span> | <span data-ttu-id="60b2d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60b2d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60b2d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60b2d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}
```
## <a name="request-headers"></a><span data-ttu-id="60b2d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60b2d-117">Request headers</span></span>
| <span data-ttu-id="60b2d-118">名前</span><span class="sxs-lookup"><span data-stu-id="60b2d-118">Name</span></span>      |<span data-ttu-id="60b2d-119">説明</span><span class="sxs-lookup"><span data-stu-id="60b2d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60b2d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b2d-120">Authorization</span></span>  | <span data-ttu-id="60b2d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60b2d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60b2d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60b2d-123">Request body</span></span>
<span data-ttu-id="60b2d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60b2d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b2d-125">応答</span><span class="sxs-lookup"><span data-stu-id="60b2d-125">Response</span></span>

<span data-ttu-id="60b2d-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、[プラン](../resources/plannerplan.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60b2d-126">If successful, this method returns a `200 OK` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="60b2d-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60b2d-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="60b2d-130">例</span><span class="sxs-lookup"><span data-stu-id="60b2d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60b2d-131">要求</span><span class="sxs-lookup"><span data-stu-id="60b2d-131">Request</span></span>
<span data-ttu-id="60b2d-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60b2d-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60b2d-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="60b2d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60b2d-134">C#</span><span class="sxs-lookup"><span data-stu-id="60b2d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60b2d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b2d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60b2d-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="60b2d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60b2d-137">応答</span><span class="sxs-lookup"><span data-stu-id="60b2d-137">Response</span></span>
<span data-ttu-id="60b2d-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="60b2d-138">Here is an example of the response.</span></span> 

><span data-ttu-id="60b2d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60b2d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
