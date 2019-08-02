---
title: conversationMembers を一覧表示する
description: チャットのメンバーを取得します。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 41bcd6211086ade6f5eb95ccc14cf53386187eec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943078"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="629d8-103">conversationMembers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="629d8-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="629d8-104">[chat](../resources/chat.md) のすべての[会話メンバー](../resources/conversationmember.md)を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="629d8-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="629d8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="629d8-105">Permissions</span></span>

<span data-ttu-id="629d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="629d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="629d8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="629d8-108">Permission Type</span></span>|<span data-ttu-id="629d8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="629d8-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="629d8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="629d8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="629d8-111">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="629d8-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="629d8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="629d8-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="629d8-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="629d8-113">Not supported</span></span>|
|<span data-ttu-id="629d8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="629d8-114">Application</span></span>| <span data-ttu-id="629d8-115">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629d8-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="629d8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="629d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="629d8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="629d8-117">Optional query parameters</span></span>

<span data-ttu-id="629d8-118">この操作は、応答をカスタマイズする [OData クエリ パラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="629d8-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="629d8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="629d8-119">Request headers</span></span>

| <span data-ttu-id="629d8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="629d8-120">Header</span></span>       | <span data-ttu-id="629d8-121">値</span><span class="sxs-lookup"><span data-stu-id="629d8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="629d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="629d8-122">Authorization</span></span>  | <span data-ttu-id="629d8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="629d8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="629d8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="629d8-125">Request body</span></span>

<span data-ttu-id="629d8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="629d8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="629d8-127">応答</span><span class="sxs-lookup"><span data-stu-id="629d8-127">Response</span></span>

<span data-ttu-id="629d8-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationMember](../resources/conversationmember.md) オブジェクトのリストを返します。</span><span class="sxs-lookup"><span data-stu-id="629d8-128">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="629d8-129">例</span><span class="sxs-lookup"><span data-stu-id="629d8-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="629d8-130">要求</span><span class="sxs-lookup"><span data-stu-id="629d8-130">Request</span></span>

<span data-ttu-id="629d8-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="629d8-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="629d8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="629d8-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="629d8-133">C#</span><span class="sxs-lookup"><span data-stu-id="629d8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="629d8-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="629d8-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="629d8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="629d8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="629d8-136">Java</span><span class="sxs-lookup"><span data-stu-id="629d8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="629d8-137">応答</span><span class="sxs-lookup"><span data-stu-id="629d8-137">Response</span></span>

<span data-ttu-id="629d8-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="629d8-138">Here is an example of the response.</span></span>

><span data-ttu-id="629d8-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="629d8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
