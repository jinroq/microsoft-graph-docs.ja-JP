---
title: Get plannerProgressTaskBoardTaskFormat
description: '**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1a8e6bbf1c56ffb966151931925572747fb5b47a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979027"
---
# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="c3592-103">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c3592-103">Get plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3592-104">**plannerProgressTaskBoardTaskFormat** オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c3592-104">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3592-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3592-105">Permissions</span></span>
<span data-ttu-id="c3592-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3592-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3592-108">Permission type</span></span>      | <span data-ttu-id="c3592-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3592-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3592-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3592-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3592-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3592-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3592-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3592-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3592-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3592-113">Not supported.</span></span>    |
|<span data-ttu-id="c3592-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3592-114">Application</span></span> | <span data-ttu-id="c3592-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3592-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3592-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3592-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="c3592-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3592-117">Request headers</span></span>
| <span data-ttu-id="c3592-118">名前</span><span class="sxs-lookup"><span data-stu-id="c3592-118">Name</span></span>      |<span data-ttu-id="c3592-119">説明</span><span class="sxs-lookup"><span data-stu-id="c3592-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3592-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3592-120">Authorization</span></span>  | <span data-ttu-id="c3592-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3592-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3592-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3592-123">Request body</span></span>
<span data-ttu-id="c3592-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3592-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3592-125">応答</span><span class="sxs-lookup"><span data-stu-id="c3592-125">Response</span></span>

<span data-ttu-id="c3592-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3592-126">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="c3592-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3592-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c3592-130">例</span><span class="sxs-lookup"><span data-stu-id="c3592-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3592-131">要求</span><span class="sxs-lookup"><span data-stu-id="c3592-131">Request</span></span>
<span data-ttu-id="c3592-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3592-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c3592-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c3592-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3592-134">C#</span><span class="sxs-lookup"><span data-stu-id="c3592-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3592-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3592-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3592-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3592-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3592-137">Java</span><span class="sxs-lookup"><span data-stu-id="c3592-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3592-138">応答</span><span class="sxs-lookup"><span data-stu-id="c3592-138">Response</span></span>
<span data-ttu-id="c3592-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3592-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
