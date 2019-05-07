---
title: 'イベント: dismissReminder'
description: ユーザーの予定表のイベントに対してトリガーされたアラームを消します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6a88e622d6f6fde60971b03ea53783d1e720512c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615500"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="89af5-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="89af5-103">event: dismissReminder</span></span>

<span data-ttu-id="89af5-104">ユーザーの[予定表](../resources/calendar.md)の[イベント](../resources/event.md)に対してトリガーされたアラームを消します。</span><span class="sxs-lookup"><span data-stu-id="89af5-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89af5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89af5-105">Permissions</span></span>
<span data-ttu-id="89af5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89af5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89af5-108">Permission type</span></span>      | <span data-ttu-id="89af5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89af5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89af5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89af5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89af5-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89af5-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="89af5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89af5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89af5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89af5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="89af5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89af5-114">Application</span></span> | <span data-ttu-id="89af5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89af5-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="89af5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89af5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="89af5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89af5-117">Request headers</span></span>
| <span data-ttu-id="89af5-118">名前</span><span class="sxs-lookup"><span data-stu-id="89af5-118">Name</span></span>       | <span data-ttu-id="89af5-119">型</span><span class="sxs-lookup"><span data-stu-id="89af5-119">Type</span></span> | <span data-ttu-id="89af5-120">説明</span><span class="sxs-lookup"><span data-stu-id="89af5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89af5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="89af5-121">Authorization</span></span>  | <span data-ttu-id="89af5-122">string</span><span class="sxs-lookup"><span data-stu-id="89af5-122">string</span></span>  | <span data-ttu-id="89af5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="89af5-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="89af5-125">応答</span><span class="sxs-lookup"><span data-stu-id="89af5-125">Response</span></span>

<span data-ttu-id="89af5-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="89af5-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89af5-128">例</span><span class="sxs-lookup"><span data-stu-id="89af5-128">Example</span></span>

<span data-ttu-id="89af5-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="89af5-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="89af5-130">要求</span><span class="sxs-lookup"><span data-stu-id="89af5-130">Request</span></span>
<span data-ttu-id="89af5-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89af5-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="89af5-132">応答</span><span class="sxs-lookup"><span data-stu-id="89af5-132">Response</span></span>
<span data-ttu-id="89af5-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="89af5-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="89af5-134">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="89af5-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89af5-135">Visual</span><span class="sxs-lookup"><span data-stu-id="89af5-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_dismissreminder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89af5-136">Java</span><span class="sxs-lookup"><span data-stu-id="89af5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_dismissreminder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-dismissreminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-dismissreminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
