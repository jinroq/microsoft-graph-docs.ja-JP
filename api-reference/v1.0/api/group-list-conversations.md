---
title: 会話の一覧表示
description: このグループの会話の一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8f400aaa5534cc660ad625f56334388770a07100
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273536"
---
# <a name="list-conversations"></a><span data-ttu-id="1a2af-103">会話の一覧表示</span><span class="sxs-lookup"><span data-stu-id="1a2af-103">List conversations</span></span>
<span data-ttu-id="1a2af-104">このグループの[会話](../resources/conversation.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a2af-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a2af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a2af-105">Permissions</span></span>
<span data-ttu-id="1a2af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a2af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a2af-108">Permission type</span></span>      | <span data-ttu-id="1a2af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a2af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a2af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a2af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a2af-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2af-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a2af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a2af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a2af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a2af-113">Not supported.</span></span>    |
|<span data-ttu-id="1a2af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a2af-114">Application</span></span> | <span data-ttu-id="1a2af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a2af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a2af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a2af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a2af-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1a2af-117">Optional query parameters</span></span>
<span data-ttu-id="1a2af-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1a2af-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a2af-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a2af-119">Request headers</span></span>
| <span data-ttu-id="1a2af-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a2af-120">Header</span></span>       | <span data-ttu-id="1a2af-121">値</span><span class="sxs-lookup"><span data-stu-id="1a2af-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a2af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a2af-122">Authorization</span></span>  | <span data-ttu-id="1a2af-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a2af-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a2af-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a2af-125">Request body</span></span>
<span data-ttu-id="1a2af-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a2af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a2af-127">応答</span><span class="sxs-lookup"><span data-stu-id="1a2af-127">Response</span></span>
<span data-ttu-id="1a2af-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Conversation](../resources/conversation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a2af-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a2af-129">例</span><span class="sxs-lookup"><span data-stu-id="1a2af-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1a2af-130">要求</span><span class="sxs-lookup"><span data-stu-id="1a2af-130">Request</span></span>
<span data-ttu-id="1a2af-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a2af-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
#### <a name="response"></a><span data-ttu-id="1a2af-132">応答</span><span class="sxs-lookup"><span data-stu-id="1a2af-132">Response</span></span>
<span data-ttu-id="1a2af-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a2af-133">The following is an example of the response.</span></span>
><span data-ttu-id="1a2af-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1a2af-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a2af-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1a2af-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a2af-137">C#</span><span class="sxs-lookup"><span data-stu-id="1a2af-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a2af-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a2af-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversations-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1a2af-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="1a2af-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversations-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-conversations.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
