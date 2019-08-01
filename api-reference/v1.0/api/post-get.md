---
title: 投稿を取得する
description: '指定したスレッド内の投稿のプロパティと関係を取得します。 親の両方を指定できます。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e6b2a5b027a6e82289ddad83877e1c61115c2233
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976028"
---
# <a name="get-post"></a><span data-ttu-id="0e2f3-104">投稿を取得する</span><span class="sxs-lookup"><span data-stu-id="0e2f3-104">Get post</span></span>

<span data-ttu-id="0e2f3-p102">指定したスレッド内の投稿のプロパティと関係を取得します。親の会話とスレッドの両方を指定したり、親の会話を参照せずにスレッドを指定したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="0e2f3-107">**投稿**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**投稿**インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e2f3-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e2f3-108">Permissions</span></span>
<span data-ttu-id="0e2f3-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e2f3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e2f3-111">Permission type</span></span>      | <span data-ttu-id="0e2f3-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e2f3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e2f3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e2f3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0e2f3-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2f3-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e2f3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e2f3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e2f3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-116">Not supported.</span></span>    |
|<span data-ttu-id="0e2f3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e2f3-117">Application</span></span> | <span data-ttu-id="0e2f3-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2f3-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e2f3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e2f3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e2f3-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0e2f3-120">Optional query parameters</span></span>
<span data-ttu-id="0e2f3-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0e2f3-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e2f3-122">Request headers</span></span>
| <span data-ttu-id="0e2f3-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e2f3-123">Header</span></span>       | <span data-ttu-id="0e2f3-124">値</span><span class="sxs-lookup"><span data-stu-id="0e2f3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e2f3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e2f3-125">Authorization</span></span>  | <span data-ttu-id="0e2f3-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e2f3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e2f3-128">Request body</span></span>
<span data-ttu-id="0e2f3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e2f3-130">応答</span><span class="sxs-lookup"><span data-stu-id="0e2f3-130">Response</span></span>

<span data-ttu-id="0e2f3-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[投稿](../resources/post.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e2f3-132">例</span><span class="sxs-lookup"><span data-stu-id="0e2f3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e2f3-133">要求</span><span class="sxs-lookup"><span data-stu-id="0e2f3-133">Request</span></span>
<span data-ttu-id="0e2f3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e2f3-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0e2f3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e2f3-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e2f3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e2f3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e2f3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e2f3-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e2f3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0e2f3-139">Java</span><span class="sxs-lookup"><span data-stu-id="0e2f3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e2f3-140">応答</span><span class="sxs-lookup"><span data-stu-id="0e2f3-140">Response</span></span>
<span data-ttu-id="0e2f3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0e2f3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="0e2f3-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e2f3-144">See also</span></span>

- [<span data-ttu-id="0e2f3-145">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="0e2f3-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0e2f3-146">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="0e2f3-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
