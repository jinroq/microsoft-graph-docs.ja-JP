---
title: イベントを削除する
description: event オブジェクトを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5973a3002b15531993e9bd2bcc1cd1615f3cdd02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965734"
---
# <a name="delete-event"></a><span data-ttu-id="985ee-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="985ee-103">Delete event</span></span>

> <span data-ttu-id="985ee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="985ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="985ee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="985ee-106">[event](../resources/event.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="985ee-106">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="985ee-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="985ee-107">Permissions</span></span>
<span data-ttu-id="985ee-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="985ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="985ee-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="985ee-110">Permission type</span></span>      | <span data-ttu-id="985ee-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="985ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="985ee-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="985ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="985ee-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="985ee-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="985ee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="985ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="985ee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ee-115">Not supported.</span></span>    |
|<span data-ttu-id="985ee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="985ee-116">Application</span></span> | <span data-ttu-id="985ee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="985ee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="985ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="985ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="985ee-119">Request headers</span></span>
| <span data-ttu-id="985ee-120">名前</span><span class="sxs-lookup"><span data-stu-id="985ee-120">Name</span></span>       | <span data-ttu-id="985ee-121">種類</span><span class="sxs-lookup"><span data-stu-id="985ee-121">Type</span></span> | <span data-ttu-id="985ee-122">説明</span><span class="sxs-lookup"><span data-stu-id="985ee-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="985ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="985ee-123">Authorization</span></span>  | <span data-ttu-id="985ee-124">string</span><span class="sxs-lookup"><span data-stu-id="985ee-124">string</span></span>  | <span data-ttu-id="985ee-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="985ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="985ee-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="985ee-127">Request body</span></span>
<span data-ttu-id="985ee-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="985ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="985ee-129">応答</span><span class="sxs-lookup"><span data-stu-id="985ee-129">Response</span></span>
<span data-ttu-id="985ee-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="985ee-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="985ee-132">例</span><span class="sxs-lookup"><span data-stu-id="985ee-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="985ee-133">要求</span><span class="sxs-lookup"><span data-stu-id="985ee-133">Request</span></span>
<span data-ttu-id="985ee-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="985ee-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="985ee-135">応答</span><span class="sxs-lookup"><span data-stu-id="985ee-135">Response</span></span>
<span data-ttu-id="985ee-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="985ee-136">The following is an example of the response.</span></span> 
><span data-ttu-id="985ee-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="985ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
