---
title: スレッドを一覧表示する
description: グループのすべてのスレッドを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 170864351673bd26e12b32b9e4337917b5321cc7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592758"
---
# <a name="list-threads"></a><span data-ttu-id="7e0d1-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7e0d1-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e0d1-104">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-104">Get all the threads of a group.</span></span>

<span data-ttu-id="7e0d1-105">注:[会話のすべてのスレッドを取得する](conversation-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e0d1-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7e0d1-106">Permissions</span></span>
<span data-ttu-id="7e0d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e0d1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e0d1-109">Permission type</span></span>      | <span data-ttu-id="7e0d1-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e0d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e0d1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e0d1-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e0d1-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e0d1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e0d1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-114">Not supported.</span></span>    |
|<span data-ttu-id="7e0d1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e0d1-115">Application</span></span> | <span data-ttu-id="7e0d1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e0d1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e0d1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e0d1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7e0d1-118">Optional query parameters</span></span>
<span data-ttu-id="7e0d1-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e0d1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0d1-120">Request headers</span></span>
| <span data-ttu-id="7e0d1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0d1-121">Header</span></span>       | <span data-ttu-id="7e0d1-122">値</span><span class="sxs-lookup"><span data-stu-id="7e0d1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e0d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e0d1-123">Authorization</span></span>  | <span data-ttu-id="7e0d1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e0d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e0d1-126">Request body</span></span>
<span data-ttu-id="7e0d1-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e0d1-128">応答</span><span class="sxs-lookup"><span data-stu-id="7e0d1-128">Response</span></span>
<span data-ttu-id="7e0d1-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e0d1-130">例</span><span class="sxs-lookup"><span data-stu-id="7e0d1-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7e0d1-131">要求</span><span class="sxs-lookup"><span data-stu-id="7e0d1-131">Request</span></span>
<span data-ttu-id="7e0d1-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="7e0d1-133">応答</span><span class="sxs-lookup"><span data-stu-id="7e0d1-133">Response</span></span>
<span data-ttu-id="7e0d1-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-134">The following is an example of the response.</span></span>
><span data-ttu-id="7e0d1-135">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e0d1-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7e0d1-136">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7e0d1-137">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="7e0d1-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7e0d1-138">Visual</span><span class="sxs-lookup"><span data-stu-id="7e0d1-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_threads-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e0d1-139">Java</span><span class="sxs-lookup"><span data-stu-id="7e0d1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_threads-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
