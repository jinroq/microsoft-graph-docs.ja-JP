---
title: List tasks
description: plannerBucket オブジェクトに関連付けられている **plannertask** オブジェクトのリストを取得します。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0760db5cf8601874cb90301bd1043522b2a102b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892116"
---
# <a name="list-tasks"></a><span data-ttu-id="5b6c3-103">List tasks</span><span class="sxs-lookup"><span data-stu-id="5b6c3-103">List tasks</span></span>

<span data-ttu-id="5b6c3-104">[plannerBucket](../resources/plannerbucket.md) オブジェクトに関連付けられている **plannertask** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-104">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b6c3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b6c3-105">Permissions</span></span>
<span data-ttu-id="5b6c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6c3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b6c3-108">Permission type</span></span>      | <span data-ttu-id="5b6c3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b6c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6c3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b6c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b6c3-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6c3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b6c3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b6c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6c3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-113">Not supported.</span></span>    |
|<span data-ttu-id="5b6c3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b6c3-114">Application</span></span> | <span data-ttu-id="5b6c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b6c3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b6c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="5b6c3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b6c3-117">Request headers</span></span>
| <span data-ttu-id="5b6c3-118">名前</span><span class="sxs-lookup"><span data-stu-id="5b6c3-118">Name</span></span>      |<span data-ttu-id="5b6c3-119">説明</span><span class="sxs-lookup"><span data-stu-id="5b6c3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b6c3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6c3-120">Authorization</span></span>  | <span data-ttu-id="5b6c3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b6c3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b6c3-123">Request body</span></span>
<span data-ttu-id="5b6c3-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6c3-125">応答</span><span class="sxs-lookup"><span data-stu-id="5b6c3-125">Response</span></span>

<span data-ttu-id="5b6c3-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerTask](../resources/plannertask.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="5b6c3-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5b6c3-130">例</span><span class="sxs-lookup"><span data-stu-id="5b6c3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b6c3-131">要求</span><span class="sxs-lookup"><span data-stu-id="5b6c3-131">Request</span></span>
<span data-ttu-id="5b6c3-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b6c3-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5b6c3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{task-id}/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b6c3-134">C#</span><span class="sxs-lookup"><span data-stu-id="5b6c3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b6c3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="5b6c3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b6c3-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="5b6c3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5b6c3-137">Java</span><span class="sxs-lookup"><span data-stu-id="5b6c3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b6c3-138">応答</span><span class="sxs-lookup"><span data-stu-id="5b6c3-138">Response</span></span>
<span data-ttu-id="5b6c3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b6c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "@odata.type": "#microsoft.graph.plannerassignment",
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
