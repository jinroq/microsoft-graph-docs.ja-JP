---
title: 会話スレッドを取得する
description: thread オブジェクトを取得します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 130c07fc00ef584b34e334f41e5eb7a6cebbdc33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843576"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="d4030-103">会話スレッドを取得する</span><span class="sxs-lookup"><span data-stu-id="d4030-103">Get conversation thread</span></span>

> <span data-ttu-id="d4030-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4030-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4030-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4030-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4030-106">[thread](../resources/conversationthread.md) オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d4030-106">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4030-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4030-107">Permissions</span></span>
<span data-ttu-id="d4030-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4030-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4030-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4030-110">Permission type</span></span>      | <span data-ttu-id="d4030-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4030-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4030-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4030-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d4030-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4030-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4030-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4030-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4030-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4030-115">Not supported.</span></span>    |
|<span data-ttu-id="d4030-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4030-116">Application</span></span> | <span data-ttu-id="d4030-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4030-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4030-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4030-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4030-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4030-119">Optional query parameters</span></span>
<span data-ttu-id="d4030-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d4030-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4030-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4030-121">Request headers</span></span>
| <span data-ttu-id="d4030-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4030-122">Header</span></span>       | <span data-ttu-id="d4030-123">値</span><span class="sxs-lookup"><span data-stu-id="d4030-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4030-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4030-124">Authorization</span></span>  | <span data-ttu-id="d4030-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4030-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4030-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4030-127">Request body</span></span>
<span data-ttu-id="d4030-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4030-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4030-129">応答</span><span class="sxs-lookup"><span data-stu-id="d4030-129">Response</span></span>
<span data-ttu-id="d4030-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [thread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4030-130">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4030-131">例</span><span class="sxs-lookup"><span data-stu-id="d4030-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4030-132">要求</span><span class="sxs-lookup"><span data-stu-id="d4030-132">Request</span></span>
<span data-ttu-id="d4030-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4030-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="d4030-134">応答</span><span class="sxs-lookup"><span data-stu-id="d4030-134">Response</span></span>
<span data-ttu-id="d4030-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4030-135">The following is an example of the response.</span></span>
><span data-ttu-id="d4030-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d4030-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
