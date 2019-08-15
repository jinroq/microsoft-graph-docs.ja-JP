---
title: 会話スレッドを取得する
description: thread オブジェクトを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ba16a2c74ec7cd63f4205061b34e6a581143e4a2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419615"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="ddedd-103">会話スレッドを取得する</span><span class="sxs-lookup"><span data-stu-id="ddedd-103">Get conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddedd-104">[thread](../resources/conversationthread.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ddedd-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddedd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddedd-105">Permissions</span></span>
<span data-ttu-id="ddedd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddedd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ddedd-108">Permission type</span></span>      | <span data-ttu-id="ddedd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ddedd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddedd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ddedd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ddedd-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddedd-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ddedd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ddedd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddedd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddedd-113">Not supported.</span></span>    |
|<span data-ttu-id="ddedd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ddedd-114">Application</span></span> | <span data-ttu-id="ddedd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddedd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddedd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ddedd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddedd-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ddedd-117">Optional query parameters</span></span>
<span data-ttu-id="ddedd-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ddedd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddedd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddedd-119">Request headers</span></span>
| <span data-ttu-id="ddedd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddedd-120">Header</span></span>       | <span data-ttu-id="ddedd-121">値</span><span class="sxs-lookup"><span data-stu-id="ddedd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ddedd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddedd-122">Authorization</span></span>  | <span data-ttu-id="ddedd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ddedd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ddedd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ddedd-125">Request body</span></span>
<span data-ttu-id="ddedd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ddedd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddedd-127">応答</span><span class="sxs-lookup"><span data-stu-id="ddedd-127">Response</span></span>
<span data-ttu-id="ddedd-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ddedd-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddedd-129">例</span><span class="sxs-lookup"><span data-stu-id="ddedd-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ddedd-130">要求</span><span class="sxs-lookup"><span data-stu-id="ddedd-130">Request</span></span>
<span data-ttu-id="ddedd-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ddedd-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ddedd-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ddedd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddedd-133">C#</span><span class="sxs-lookup"><span data-stu-id="ddedd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddedd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddedd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddedd-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="ddedd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddedd-136">応答</span><span class="sxs-lookup"><span data-stu-id="ddedd-136">Response</span></span>
<span data-ttu-id="ddedd-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ddedd-137">The following is an example of the response.</span></span>
><span data-ttu-id="ddedd-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ddedd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
