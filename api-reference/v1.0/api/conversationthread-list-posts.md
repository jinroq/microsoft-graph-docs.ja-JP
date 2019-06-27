---
title: 投稿を一覧表示する
description: '指定したスレッドの投稿を取得します。 親の会話とスレッドの両方を指定できます。または、 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: cd0943addbd95eddb876b6fd0476542ad830cbec
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276427"
---
# <a name="list-posts"></a><span data-ttu-id="9af23-104">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9af23-104">List posts</span></span>

<span data-ttu-id="9af23-p102">指定したスレッドの投稿を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="9af23-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9af23-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9af23-107">Permissions</span></span>
<span data-ttu-id="9af23-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9af23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af23-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9af23-110">Permission type</span></span>      | <span data-ttu-id="9af23-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9af23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af23-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9af23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9af23-113">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="9af23-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="9af23-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9af23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9af23-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9af23-115">Not supported.</span></span>    |
|<span data-ttu-id="9af23-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9af23-116">Application</span></span> | <span data-ttu-id="9af23-117">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="9af23-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af23-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9af23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="9af23-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9af23-119">Optional query parameters</span></span>
<span data-ttu-id="9af23-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9af23-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9af23-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9af23-121">Request headers</span></span>
| <span data-ttu-id="9af23-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9af23-122">Header</span></span>       | <span data-ttu-id="9af23-123">値</span><span class="sxs-lookup"><span data-stu-id="9af23-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9af23-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9af23-124">Authorization</span></span>  | <span data-ttu-id="9af23-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9af23-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9af23-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9af23-127">Request body</span></span>
<span data-ttu-id="9af23-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9af23-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9af23-129">応答</span><span class="sxs-lookup"><span data-stu-id="9af23-129">Response</span></span>

<span data-ttu-id="9af23-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Post](../resources/post.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9af23-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9af23-131">例</span><span class="sxs-lookup"><span data-stu-id="9af23-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9af23-132">要求</span><span class="sxs-lookup"><span data-stu-id="9af23-132">Request</span></span>
<span data-ttu-id="9af23-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9af23-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="9af23-134">応答</span><span class="sxs-lookup"><span data-stu-id="9af23-134">Response</span></span>
<span data-ttu-id="9af23-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9af23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9af23-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9af23-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9af23-139">C#</span><span class="sxs-lookup"><span data-stu-id="9af23-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_posts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9af23-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="9af23-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_posts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9af23-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="9af23-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_posts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversationthread-list-posts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/conversationthread-list-posts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversationthread-list-posts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
