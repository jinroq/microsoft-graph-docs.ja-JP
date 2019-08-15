---
title: conversationMember を取得する
description: チャットのメンバーを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ff0ec4dfd39c4f5d2c54be567869d23f362eb87
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417825"
---
# <a name="get-conversationmember"></a><span data-ttu-id="ff557-103">conversationMember を取得する</span><span class="sxs-lookup"><span data-stu-id="ff557-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff557-104">[chat](../resources/chat.md) から [conversationMember](../resources/conversationmember.md) を取得します。</span><span class="sxs-lookup"><span data-stu-id="ff557-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff557-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff557-105">Permissions</span></span>

<span data-ttu-id="ff557-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff557-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff557-108">Permission Type</span></span>|<span data-ttu-id="ff557-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff557-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ff557-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff557-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ff557-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff557-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="ff557-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff557-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff557-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="ff557-113">Not supported</span></span>|
|<span data-ttu-id="ff557-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff557-114">Application</span></span> |<span data-ttu-id="ff557-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff557-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff557-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff557-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff557-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff557-117">Optional query parameters</span></span>

<span data-ttu-id="ff557-118">この操作は、応答をカスタマイズする [OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="ff557-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff557-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff557-119">Request headers</span></span>

| <span data-ttu-id="ff557-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff557-120">Header</span></span>       | <span data-ttu-id="ff557-121">値</span><span class="sxs-lookup"><span data-stu-id="ff557-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff557-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff557-122">Authorization</span></span>  | <span data-ttu-id="ff557-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff557-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff557-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff557-125">Request body</span></span>

<span data-ttu-id="ff557-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff557-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff557-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff557-127">Response</span></span>

<span data-ttu-id="ff557-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[conversationMember](../resources/conversationmember.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff557-128">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff557-129">例</span><span class="sxs-lookup"><span data-stu-id="ff557-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ff557-130">要求</span><span class="sxs-lookup"><span data-stu-id="ff557-130">Request</span></span>

<span data-ttu-id="ff557-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff557-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff557-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff557-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff557-133">C#</span><span class="sxs-lookup"><span data-stu-id="ff557-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff557-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff557-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff557-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff557-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff557-136">応答</span><span class="sxs-lookup"><span data-stu-id="ff557-136">Response</span></span>

<span data-ttu-id="ff557-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ff557-137">Here is an example of the response.</span></span> 

><span data-ttu-id="ff557-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff557-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
