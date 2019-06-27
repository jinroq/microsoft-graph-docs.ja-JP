---
title: conversationMember を取得する
description: チャットのメンバーを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3b9fddad9b3378b5e4e6df3fd571b070d71900e3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261125"
---
# <a name="get-conversationmember"></a><span data-ttu-id="808ea-103">conversationMember を取得する</span><span class="sxs-lookup"><span data-stu-id="808ea-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="808ea-104">[chat](../resources/chat.md) から [conversationMember](../resources/conversationmember.md) を取得します。</span><span class="sxs-lookup"><span data-stu-id="808ea-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="808ea-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="808ea-105">Permissions</span></span>

<span data-ttu-id="808ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="808ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="808ea-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="808ea-108">Permission Type</span></span>|<span data-ttu-id="808ea-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="808ea-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="808ea-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="808ea-110">Delegated (work or school account)</span></span>|<span data-ttu-id="808ea-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="808ea-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="808ea-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="808ea-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="808ea-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="808ea-113">Not supported</span></span>|
|<span data-ttu-id="808ea-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="808ea-114">Application</span></span> |<span data-ttu-id="808ea-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="808ea-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="808ea-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="808ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="808ea-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="808ea-117">Optional query parameters</span></span>

<span data-ttu-id="808ea-118">この操作は、応答をカスタマイズする [OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="808ea-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="808ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="808ea-119">Request headers</span></span>

| <span data-ttu-id="808ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="808ea-120">Header</span></span>       | <span data-ttu-id="808ea-121">値</span><span class="sxs-lookup"><span data-stu-id="808ea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="808ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="808ea-122">Authorization</span></span>  | <span data-ttu-id="808ea-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="808ea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="808ea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="808ea-125">Request body</span></span>

<span data-ttu-id="808ea-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="808ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="808ea-127">応答</span><span class="sxs-lookup"><span data-stu-id="808ea-127">Response</span></span>

<span data-ttu-id="808ea-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[conversationMember](../resources/conversationmember.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="808ea-128">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="808ea-129">例</span><span class="sxs-lookup"><span data-stu-id="808ea-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="808ea-130">要求</span><span class="sxs-lookup"><span data-stu-id="808ea-130">Request</span></span>

<span data-ttu-id="808ea-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="808ea-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="808ea-132">応答</span><span class="sxs-lookup"><span data-stu-id="808ea-132">Response</span></span>

<span data-ttu-id="808ea-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="808ea-133">Here is an example of the response.</span></span> 

><span data-ttu-id="808ea-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="808ea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="808ea-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="808ea-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="808ea-137">C#</span><span class="sxs-lookup"><span data-stu-id="808ea-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="808ea-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="808ea-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="808ea-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="808ea-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversation_member-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
