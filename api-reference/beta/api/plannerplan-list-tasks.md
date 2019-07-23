---
title: List tasks
description: Plan オブジェクトに関連**** 付けられているプランのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: cdffe20f835a0cea1166e6111a69a84e85c8d645
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820753"
---
# <a name="list-tasks"></a><span data-ttu-id="bafb7-103">タスクを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bafb7-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafb7-104">Plan オブジェクトに関連[](../resources/plannertask.md)付けられている[プラン](../resources/plannerplan.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="bafb7-104">Retrieve a list of [plannerTask](../resources/plannertask.md) objects associated with a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bafb7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bafb7-105">Permissions</span></span>
<span data-ttu-id="bafb7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bafb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bafb7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bafb7-108">Permission type</span></span>      | <span data-ttu-id="bafb7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bafb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bafb7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bafb7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bafb7-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafb7-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bafb7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bafb7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bafb7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bafb7-113">Not supported.</span></span>    |
|<span data-ttu-id="bafb7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bafb7-114">Application</span></span> | <span data-ttu-id="bafb7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bafb7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bafb7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bafb7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="bafb7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bafb7-117">Request headers</span></span>
| <span data-ttu-id="bafb7-118">名前</span><span class="sxs-lookup"><span data-stu-id="bafb7-118">Name</span></span>      |<span data-ttu-id="bafb7-119">説明</span><span class="sxs-lookup"><span data-stu-id="bafb7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bafb7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bafb7-120">Authorization</span></span>  | <span data-ttu-id="bafb7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bafb7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bafb7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bafb7-123">Request body</span></span>
<span data-ttu-id="bafb7-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bafb7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bafb7-125">応答</span><span class="sxs-lookup"><span data-stu-id="bafb7-125">Response</span></span>

<span data-ttu-id="bafb7-126">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、[プランの task](../resources/plannertask.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bafb7-126">If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="bafb7-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bafb7-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bafb7-130">例</span><span class="sxs-lookup"><span data-stu-id="bafb7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bafb7-131">要求</span><span class="sxs-lookup"><span data-stu-id="bafb7-131">Request</span></span>
<span data-ttu-id="bafb7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bafb7-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bafb7-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bafb7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bafb7-134">C#</span><span class="sxs-lookup"><span data-stu-id="bafb7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bafb7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bafb7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bafb7-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="bafb7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bafb7-137">応答</span><span class="sxs-lookup"><span data-stu-id="bafb7-137">Response</span></span>
<span data-ttu-id="bafb7-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bafb7-138">Here is an example of the response.</span></span> 

><span data-ttu-id="bafb7-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="bafb7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
