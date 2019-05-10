---
title: チャットの取得
description: 1 つのチャットを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 19fce3e08788611cdbb03b7c70eb94753c5f7680
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591638"
---
# <a name="get-chat"></a><span data-ttu-id="5bee2-103">チャットの取得</span><span class="sxs-lookup"><span data-stu-id="5bee2-103">Get chat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bee2-104">1 つの[チャット](../resources/chat.md)を取得します (メッセージなし)。</span><span class="sxs-lookup"><span data-stu-id="5bee2-104">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bee2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bee2-105">Permissions</span></span>

<span data-ttu-id="5bee2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bee2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bee2-108">Permission type</span></span>      | <span data-ttu-id="5bee2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bee2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bee2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bee2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bee2-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="5bee2-111">Chat.Read</span></span>   |
|<span data-ttu-id="5bee2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bee2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bee2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bee2-113">Not supported.</span></span>    |
|<span data-ttu-id="5bee2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bee2-114">Application</span></span> | <span data-ttu-id="5bee2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bee2-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="5bee2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bee2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bee2-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5bee2-117">Optional query parameters</span></span>

<span data-ttu-id="5bee2-118">この操作は現在、応答をカスタマイズする[OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="5bee2-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bee2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bee2-119">Request headers</span></span>

| <span data-ttu-id="5bee2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bee2-120">Header</span></span>       | <span data-ttu-id="5bee2-121">値</span><span class="sxs-lookup"><span data-stu-id="5bee2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5bee2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bee2-122">Authorization</span></span>  | <span data-ttu-id="5bee2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bee2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5bee2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bee2-125">Request body</span></span>

<span data-ttu-id="5bee2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5bee2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bee2-127">応答</span><span class="sxs-lookup"><span data-stu-id="5bee2-127">Response</span></span>

<span data-ttu-id="5bee2-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chat](../resources/chat.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5bee2-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bee2-129">例</span><span class="sxs-lookup"><span data-stu-id="5bee2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bee2-130">要求</span><span class="sxs-lookup"><span data-stu-id="5bee2-130">Request</span></span>
<span data-ttu-id="5bee2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bee2-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```

##### <a name="response"></a><span data-ttu-id="5bee2-132">応答</span><span class="sxs-lookup"><span data-stu-id="5bee2-132">Response</span></span>
<span data-ttu-id="5bee2-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5bee2-133">Here is an example of the response.</span></span> 

><span data-ttu-id="5bee2-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5bee2-134">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="5bee2-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5bee2-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bee2-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5bee2-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bee2-137">C#</span><span class="sxs-lookup"><span data-stu-id="5bee2-137">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chat_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bee2-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bee2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chat_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chat-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
