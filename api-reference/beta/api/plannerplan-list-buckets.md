---
title: List buckets
description: plannerPlan オブジェクトに含まれている **plannerbucket** オブジェクトのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b2722ea6f6c30c185579fe3afa42e54d1444a68d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876432"
---
# <a name="list-buckets"></a><span data-ttu-id="dab12-103">List buckets</span><span class="sxs-lookup"><span data-stu-id="dab12-103">List buckets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dab12-104">Plan オブジェクトに含ま[](../resources/plannerbucket.md)れている plan オブジェクトの一覧[](../resources/plannerplan.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="dab12-104">Retrieve a list of [plannerBucket](../resources/plannerbucket.md) objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dab12-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dab12-105">Permissions</span></span>
<span data-ttu-id="dab12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab12-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dab12-108">Permission type</span></span>      | <span data-ttu-id="dab12-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dab12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab12-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dab12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dab12-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab12-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dab12-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dab12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dab12-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab12-113">Not supported.</span></span>    |
|<span data-ttu-id="dab12-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dab12-114">Application</span></span> | <span data-ttu-id="dab12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dab12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dab12-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dab12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="dab12-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dab12-117">Request headers</span></span>
| <span data-ttu-id="dab12-118">名前</span><span class="sxs-lookup"><span data-stu-id="dab12-118">Name</span></span>      |<span data-ttu-id="dab12-119">説明</span><span class="sxs-lookup"><span data-stu-id="dab12-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dab12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab12-120">Authorization</span></span>  | <span data-ttu-id="dab12-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dab12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dab12-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dab12-123">Request body</span></span>
<span data-ttu-id="dab12-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dab12-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dab12-125">応答</span><span class="sxs-lookup"><span data-stu-id="dab12-125">Response</span></span>

<span data-ttu-id="dab12-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[plan/バケツ](../resources/plannerbucket.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dab12-126">If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="dab12-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dab12-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="dab12-130">例</span><span class="sxs-lookup"><span data-stu-id="dab12-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dab12-131">要求</span><span class="sxs-lookup"><span data-stu-id="dab12-131">Request</span></span>
<span data-ttu-id="dab12-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dab12-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dab12-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dab12-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dab12-134">C#</span><span class="sxs-lookup"><span data-stu-id="dab12-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dab12-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="dab12-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dab12-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="dab12-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dab12-137">Java</span><span class="sxs-lookup"><span data-stu-id="dab12-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dab12-138">応答</span><span class="sxs-lookup"><span data-stu-id="dab12-138">Response</span></span>
<span data-ttu-id="dab12-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dab12-139">Here is an example of the response.</span></span> 

><span data-ttu-id="dab12-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="dab12-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
