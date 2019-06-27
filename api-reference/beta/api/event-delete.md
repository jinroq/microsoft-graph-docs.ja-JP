---
title: イベントの削除
description: イベントを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 82bcfd5b8db1932f855fd399159824f0d3cf89c8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259172"
---
# <a name="delete-event"></a><span data-ttu-id="ce9d9-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="ce9d9-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce9d9-104">イベントを削除します。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce9d9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce9d9-105">Permissions</span></span>
<span data-ttu-id="ce9d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce9d9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce9d9-108">Permission type</span></span>      | <span data-ttu-id="ce9d9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce9d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce9d9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce9d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce9d9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce9d9-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ce9d9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce9d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce9d9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce9d9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ce9d9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce9d9-114">Application</span></span> | <span data-ttu-id="ce9d9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce9d9-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce9d9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce9d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce9d9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce9d9-117">Request headers</span></span>
| <span data-ttu-id="ce9d9-118">名前</span><span class="sxs-lookup"><span data-stu-id="ce9d9-118">Name</span></span>       | <span data-ttu-id="ce9d9-119">型</span><span class="sxs-lookup"><span data-stu-id="ce9d9-119">Type</span></span> | <span data-ttu-id="ce9d9-120">説明</span><span class="sxs-lookup"><span data-stu-id="ce9d9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce9d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce9d9-121">Authorization</span></span>  | <span data-ttu-id="ce9d9-122">string</span><span class="sxs-lookup"><span data-stu-id="ce9d9-122">string</span></span>  | <span data-ttu-id="ce9d9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce9d9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce9d9-125">Request body</span></span>
<span data-ttu-id="ce9d9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce9d9-127">応答</span><span class="sxs-lookup"><span data-stu-id="ce9d9-127">Response</span></span>

<span data-ttu-id="ce9d9-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce9d9-130">例</span><span class="sxs-lookup"><span data-stu-id="ce9d9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce9d9-131">要求</span><span class="sxs-lookup"><span data-stu-id="ce9d9-131">Request</span></span>
<span data-ttu-id="ce9d9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="ce9d9-133">応答</span><span class="sxs-lookup"><span data-stu-id="ce9d9-133">Response</span></span>
<span data-ttu-id="ce9d9-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ce9d9-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce9d9-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ce9d9-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce9d9-136">C#</span><span class="sxs-lookup"><span data-stu-id="ce9d9-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce9d9-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce9d9-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_event-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce9d9-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="ce9d9-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_event-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
