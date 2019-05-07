---
title: スレッドを一覧表示する
description: グループのすべてのスレッドを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 40ddb78e3aeb1334e2fd9990242503b62d0c2448
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614076"
---
# <a name="list-threads"></a><span data-ttu-id="c2a45-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c2a45-103">List threads</span></span>
<span data-ttu-id="c2a45-104">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="c2a45-104">Get all the threads of a group.</span></span>

><span data-ttu-id="c2a45-105">注:[会話のすべてのスレッドを取得する](conversation-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="c2a45-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2a45-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2a45-106">Permissions</span></span>
<span data-ttu-id="c2a45-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2a45-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2a45-109">Permission type</span></span>      | <span data-ttu-id="c2a45-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2a45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2a45-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2a45-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a45-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2a45-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2a45-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a45-114">Not supported.</span></span>    |
|<span data-ttu-id="c2a45-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2a45-115">Application</span></span> | <span data-ttu-id="c2a45-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a45-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2a45-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2a45-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2a45-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2a45-118">Optional query parameters</span></span>
<span data-ttu-id="c2a45-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c2a45-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2a45-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a45-120">Request headers</span></span>
| <span data-ttu-id="c2a45-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a45-121">Header</span></span>       | <span data-ttu-id="c2a45-122">値</span><span class="sxs-lookup"><span data-stu-id="c2a45-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2a45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2a45-123">Authorization</span></span>  | <span data-ttu-id="c2a45-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2a45-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2a45-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2a45-126">Request body</span></span>
<span data-ttu-id="c2a45-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c2a45-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2a45-128">応答</span><span class="sxs-lookup"><span data-stu-id="c2a45-128">Response</span></span>
<span data-ttu-id="c2a45-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ConversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c2a45-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2a45-130">例</span><span class="sxs-lookup"><span data-stu-id="c2a45-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c2a45-131">要求</span><span class="sxs-lookup"><span data-stu-id="c2a45-131">Request</span></span>
<span data-ttu-id="c2a45-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2a45-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="c2a45-133">応答</span><span class="sxs-lookup"><span data-stu-id="c2a45-133">Response</span></span>
<span data-ttu-id="c2a45-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2a45-134">The following is an example of the response.</span></span>
><span data-ttu-id="c2a45-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c2a45-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2a45-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="c2a45-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2a45-138">Visual</span><span class="sxs-lookup"><span data-stu-id="c2a45-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_threads-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2a45-139">Java</span><span class="sxs-lookup"><span data-stu-id="c2a45-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_threads-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
