---
title: 会話スレッドを取得する
description: thread オブジェクトを取得します。
author: dkershaw10
ms.openlocfilehash: 615a606bbe0e58da233642c55baccb3f05dc3dd6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347727"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="c22ba-103">会話スレッドを取得する</span><span class="sxs-lookup"><span data-stu-id="c22ba-103">Get conversation thread</span></span>

> <span data-ttu-id="c22ba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c22ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c22ba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c22ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c22ba-106">[thread](../resources/conversationthread.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c22ba-106">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c22ba-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c22ba-107">Permissions</span></span>
<span data-ttu-id="c22ba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c22ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c22ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c22ba-110">Permission type</span></span>      | <span data-ttu-id="c22ba-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c22ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c22ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c22ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c22ba-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22ba-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c22ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c22ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c22ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c22ba-115">Not supported.</span></span>    |
|<span data-ttu-id="c22ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c22ba-116">Application</span></span> | <span data-ttu-id="c22ba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c22ba-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c22ba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c22ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c22ba-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c22ba-119">Optional query parameters</span></span>
<span data-ttu-id="c22ba-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c22ba-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c22ba-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c22ba-121">Request headers</span></span>
| <span data-ttu-id="c22ba-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c22ba-122">Header</span></span>       | <span data-ttu-id="c22ba-123">値</span><span class="sxs-lookup"><span data-stu-id="c22ba-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c22ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c22ba-124">Authorization</span></span>  | <span data-ttu-id="c22ba-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c22ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c22ba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c22ba-127">Request body</span></span>
<span data-ttu-id="c22ba-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c22ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c22ba-129">応答</span><span class="sxs-lookup"><span data-stu-id="c22ba-129">Response</span></span>
<span data-ttu-id="c22ba-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c22ba-130">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c22ba-131">例</span><span class="sxs-lookup"><span data-stu-id="c22ba-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c22ba-132">要求</span><span class="sxs-lookup"><span data-stu-id="c22ba-132">Request</span></span>
<span data-ttu-id="c22ba-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c22ba-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="c22ba-134">応答</span><span class="sxs-lookup"><span data-stu-id="c22ba-134">Response</span></span>
<span data-ttu-id="c22ba-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c22ba-135">The following is an example of the response.</span></span>
><span data-ttu-id="c22ba-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c22ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->