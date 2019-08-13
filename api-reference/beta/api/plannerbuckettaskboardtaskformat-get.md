---
title: Get plannerBucketTaskBoardTaskFormat
description: '**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 93c33a32cdcc7395a21d92564ccdddb809444f0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348103"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="e1455-103">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e1455-103">Get plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1455-104">**plannerBucketTaskBoardTaskFormat** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="e1455-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1455-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e1455-105">Permissions</span></span>
<span data-ttu-id="e1455-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1455-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1455-108">Permission type</span></span>      | <span data-ttu-id="e1455-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1455-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1455-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1455-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1455-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1455-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1455-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1455-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1455-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1455-113">Not supported.</span></span>    |
|<span data-ttu-id="e1455-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1455-114">Application</span></span> | <span data-ttu-id="e1455-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1455-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1455-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1455-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="e1455-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1455-117">Request headers</span></span>
| <span data-ttu-id="e1455-118">名前</span><span class="sxs-lookup"><span data-stu-id="e1455-118">Name</span></span>      |<span data-ttu-id="e1455-119">説明</span><span class="sxs-lookup"><span data-stu-id="e1455-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1455-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1455-120">Authorization</span></span>  | <span data-ttu-id="e1455-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e1455-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1455-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1455-123">Request body</span></span>
<span data-ttu-id="e1455-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e1455-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1455-125">応答</span><span class="sxs-lookup"><span data-stu-id="e1455-125">Response</span></span>

<span data-ttu-id="e1455-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1455-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e1455-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1455-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e1455-130">例</span><span class="sxs-lookup"><span data-stu-id="e1455-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1455-131">要求</span><span class="sxs-lookup"><span data-stu-id="e1455-131">Request</span></span>
<span data-ttu-id="e1455-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1455-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1455-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e1455-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1455-134">C#</span><span class="sxs-lookup"><span data-stu-id="e1455-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerbuckettaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1455-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1455-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerbuckettaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1455-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e1455-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerbuckettaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e1455-137">Java</span><span class="sxs-lookup"><span data-stu-id="e1455-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerbuckettaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e1455-138">応答</span><span class="sxs-lookup"><span data-stu-id="e1455-138">Response</span></span>
<span data-ttu-id="e1455-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1455-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
