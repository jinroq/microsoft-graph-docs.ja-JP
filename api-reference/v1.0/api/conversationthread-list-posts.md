---
title: 投稿を一覧表示する
description: '指定したスレッドの投稿を取得します。 親スレッドと、スレッドの両方を指定することができますか、 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: aa411939f9e8040b127a8821c23b557defffbaec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961520"
---
# <a name="list-posts"></a><span data-ttu-id="f0808-104">投稿を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0808-104">List posts</span></span>

<span data-ttu-id="f0808-p102">指定したスレッドの投稿を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0808-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0808-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0808-107">Permissions</span></span>
<span data-ttu-id="f0808-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0808-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0808-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0808-110">Permission type</span></span>      | <span data-ttu-id="f0808-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0808-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0808-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0808-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0808-113">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0808-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="f0808-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0808-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0808-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0808-115">Not supported.</span></span>    |
|<span data-ttu-id="f0808-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0808-116">Application</span></span> | <span data-ttu-id="f0808-117">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0808-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0808-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0808-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0808-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0808-119">Optional query parameters</span></span>
<span data-ttu-id="f0808-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0808-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0808-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0808-121">Request headers</span></span>
| <span data-ttu-id="f0808-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0808-122">Header</span></span>       | <span data-ttu-id="f0808-123">値</span><span class="sxs-lookup"><span data-stu-id="f0808-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0808-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0808-124">Authorization</span></span>  | <span data-ttu-id="f0808-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0808-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0808-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0808-127">Request body</span></span>
<span data-ttu-id="f0808-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0808-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0808-129">応答</span><span class="sxs-lookup"><span data-stu-id="f0808-129">Response</span></span>

<span data-ttu-id="f0808-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Post](../resources/post.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f0808-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0808-131">例</span><span class="sxs-lookup"><span data-stu-id="f0808-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0808-132">要求</span><span class="sxs-lookup"><span data-stu-id="f0808-132">Request</span></span>
<span data-ttu-id="f0808-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0808-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="f0808-134">応答</span><span class="sxs-lookup"><span data-stu-id="f0808-134">Response</span></span>
<span data-ttu-id="f0808-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0808-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
