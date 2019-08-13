---
title: チャットの一覧表示
description: ユーザーのチャットのリストを取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: be9e3f5e5cf40465b4f7bc4614ca9a2074eaaa58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320008"
---
# <a name="list-chats"></a><span data-ttu-id="728c3-103">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="728c3-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="728c3-104">ユーザーが所属している[チャット](../resources/chat.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="728c3-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="728c3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="728c3-105">Permissions</span></span>

<span data-ttu-id="728c3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="728c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="728c3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="728c3-108">Permission type</span></span>      | <span data-ttu-id="728c3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="728c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="728c3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="728c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="728c3-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="728c3-111">Chat.Read</span></span>   |
|<span data-ttu-id="728c3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="728c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="728c3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="728c3-113">Not supported.</span></span>    |
|<span data-ttu-id="728c3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="728c3-114">Application</span></span> | <span data-ttu-id="728c3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="728c3-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="728c3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="728c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="728c3-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="728c3-117">Optional query parameters</span></span>

<span data-ttu-id="728c3-118">この操作は現在、応答をカスタマイズする[OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="728c3-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="728c3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="728c3-119">Request headers</span></span>

| <span data-ttu-id="728c3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="728c3-120">Header</span></span>       | <span data-ttu-id="728c3-121">値</span><span class="sxs-lookup"><span data-stu-id="728c3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="728c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="728c3-122">Authorization</span></span>  | <span data-ttu-id="728c3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="728c3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="728c3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="728c3-125">Request body</span></span>

<span data-ttu-id="728c3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="728c3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="728c3-127">応答</span><span class="sxs-lookup"><span data-stu-id="728c3-127">Response</span></span>

<span data-ttu-id="728c3-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chat](../resources/chat.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="728c3-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="728c3-129">例</span><span class="sxs-lookup"><span data-stu-id="728c3-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="728c3-130">要求</span><span class="sxs-lookup"><span data-stu-id="728c3-130">Request</span></span>

<span data-ttu-id="728c3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="728c3-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="728c3-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="728c3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="728c3-133">C#</span><span class="sxs-lookup"><span data-stu-id="728c3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="728c3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="728c3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="728c3-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="728c3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="728c3-136">Java</span><span class="sxs-lookup"><span data-stu-id="728c3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="728c3-137">応答</span><span class="sxs-lookup"><span data-stu-id="728c3-137">Response</span></span>

<span data-ttu-id="728c3-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="728c3-138">Here is an example of the response.</span></span> 

><span data-ttu-id="728c3-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="728c3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "value": [
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:51:42.099Z",
            "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_0c5cfdbb-596f-4d39-b557-5d9516c94107@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:19:23.76Z",
            "lastUpdatedDateTime": "2019-04-18T23:19:21.994Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_3ee373aa-62fa-4fc6-b11f-9627d5b4a73d@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-03-21T22:30:14.867Z",
            "lastUpdatedDateTime": "2019-03-21T22:30:15.507Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_90a27c51-5c74-453b-944a-134ba86da790@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-02-06T03:38:58.062Z",
            "lastUpdatedDateTime": "2019-02-06T03:38:58.063Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
