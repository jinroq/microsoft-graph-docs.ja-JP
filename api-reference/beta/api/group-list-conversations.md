---
title: 会話の一覧表示
description: このグループの会話の一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 4ef148acd4a3d98a0e5d9c3ad75b5ab3cd0d1489
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823843"
---
# <a name="list-conversations"></a><span data-ttu-id="de315-103">会話の一覧表示</span><span class="sxs-lookup"><span data-stu-id="de315-103">List conversations</span></span>

> <span data-ttu-id="de315-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de315-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de315-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de315-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de315-106">このグループの[会話](../resources/conversation.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="de315-106">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="de315-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de315-107">Permissions</span></span>
<span data-ttu-id="de315-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de315-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de315-110">Permission type</span></span>      | <span data-ttu-id="de315-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de315-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de315-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de315-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de315-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de315-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="de315-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de315-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de315-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de315-115">Not supported.</span></span>    |
|<span data-ttu-id="de315-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de315-116">Application</span></span> | <span data-ttu-id="de315-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de315-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de315-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de315-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de315-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="de315-119">Optional query parameters</span></span>
<span data-ttu-id="de315-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="de315-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de315-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de315-121">Request headers</span></span>
| <span data-ttu-id="de315-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de315-122">Header</span></span>       | <span data-ttu-id="de315-123">値</span><span class="sxs-lookup"><span data-stu-id="de315-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de315-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="de315-124">Authorization</span></span>  | <span data-ttu-id="de315-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de315-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de315-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="de315-127">Request body</span></span>
<span data-ttu-id="de315-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="de315-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de315-129">応答</span><span class="sxs-lookup"><span data-stu-id="de315-129">Response</span></span>
<span data-ttu-id="de315-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Conversation](../resources/conversation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="de315-130">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de315-131">例</span><span class="sxs-lookup"><span data-stu-id="de315-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="de315-132">要求</span><span class="sxs-lookup"><span data-stu-id="de315-132">Request</span></span>
<span data-ttu-id="de315-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de315-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```

#### <a name="response"></a><span data-ttu-id="de315-134">応答</span><span class="sxs-lookup"><span data-stu-id="de315-134">Response</span></span>
<span data-ttu-id="de315-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de315-135">The following is an example of the response.</span></span>
><span data-ttu-id="de315-136">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="de315-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="de315-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="de315-137">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
