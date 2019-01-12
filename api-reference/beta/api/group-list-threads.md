---
title: スレッドを一覧表示する
description: グループのすべてのスレッドを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a79a6fc2568ae550d2323a401c4e0fd22b6d9b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984501"
---
# <a name="list-threads"></a><span data-ttu-id="cef84-103">スレッドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cef84-103">List threads</span></span>

> <span data-ttu-id="cef84-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cef84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cef84-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cef84-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cef84-106">グループのすべてのスレッドを取得します。</span><span class="sxs-lookup"><span data-stu-id="cef84-106">Get all the threads of a group.</span></span>

<span data-ttu-id="cef84-107">注:[会話のすべてのスレッドを取得する](conversation-list-threads.md)ことも可能です。</span><span class="sxs-lookup"><span data-stu-id="cef84-107">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cef84-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cef84-108">Permissions</span></span>
<span data-ttu-id="cef84-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cef84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef84-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cef84-111">Permission type</span></span>      | <span data-ttu-id="cef84-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cef84-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cef84-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cef84-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cef84-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef84-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cef84-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cef84-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef84-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cef84-116">Not supported.</span></span>    |
|<span data-ttu-id="cef84-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cef84-117">Application</span></span> | <span data-ttu-id="cef84-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cef84-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cef84-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cef84-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cef84-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cef84-120">Optional query parameters</span></span>
<span data-ttu-id="cef84-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cef84-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cef84-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cef84-122">Request headers</span></span>
| <span data-ttu-id="cef84-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cef84-123">Header</span></span>       | <span data-ttu-id="cef84-124">値</span><span class="sxs-lookup"><span data-stu-id="cef84-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cef84-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef84-125">Authorization</span></span>  | <span data-ttu-id="cef84-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cef84-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cef84-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="cef84-128">Request body</span></span>
<span data-ttu-id="cef84-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cef84-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cef84-130">応答</span><span class="sxs-lookup"><span data-stu-id="cef84-130">Response</span></span>
<span data-ttu-id="cef84-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [conversationThread](../resources/conversationthread.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cef84-131">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cef84-132">例</span><span class="sxs-lookup"><span data-stu-id="cef84-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cef84-133">要求</span><span class="sxs-lookup"><span data-stu-id="cef84-133">Request</span></span>
<span data-ttu-id="cef84-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cef84-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="cef84-135">応答</span><span class="sxs-lookup"><span data-stu-id="cef84-135">Response</span></span>
<span data-ttu-id="cef84-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cef84-136">The following is an example of the response.</span></span>
><span data-ttu-id="cef84-137">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cef84-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cef84-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cef84-138">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
