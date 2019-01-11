---
title: 'イベント: dismissReminder'
description: ユーザーの予定表でイベントをトリガーされたアラームを閉じます。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 570a9b34031afe6d53b6e577127180ebdbe7a163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864940"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="f490b-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="f490b-103">event: dismissReminder</span></span>

> <span data-ttu-id="f490b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f490b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f490b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f490b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f490b-106">ユーザー[の予定表](../resources/calendar.md)の[イベント](../resources/event.md)のトリガーされたアラームを閉じます。</span><span class="sxs-lookup"><span data-stu-id="f490b-106">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f490b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f490b-107">Permissions</span></span>
<span data-ttu-id="f490b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f490b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f490b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f490b-110">Permission type</span></span>      | <span data-ttu-id="f490b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f490b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f490b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f490b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f490b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f490b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f490b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f490b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f490b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f490b-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f490b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f490b-116">Application</span></span> | <span data-ttu-id="f490b-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f490b-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f490b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f490b-118">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f490b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f490b-119">Request headers</span></span>

| <span data-ttu-id="f490b-120">名前</span><span class="sxs-lookup"><span data-stu-id="f490b-120">Name</span></span>       | <span data-ttu-id="f490b-121">種類</span><span class="sxs-lookup"><span data-stu-id="f490b-121">Type</span></span> | <span data-ttu-id="f490b-122">説明</span><span class="sxs-lookup"><span data-stu-id="f490b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f490b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f490b-123">Authorization</span></span>  | <span data-ttu-id="f490b-124">string</span><span class="sxs-lookup"><span data-stu-id="f490b-124">string</span></span>  | <span data-ttu-id="f490b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f490b-p103">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="f490b-127">応答</span><span class="sxs-lookup"><span data-stu-id="f490b-127">Response</span></span>

<span data-ttu-id="f490b-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f490b-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f490b-130">例</span><span class="sxs-lookup"><span data-stu-id="f490b-130">Example</span></span>

<span data-ttu-id="f490b-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f490b-131">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f490b-132">要求</span><span class="sxs-lookup"><span data-stu-id="f490b-132">Request</span></span>
<span data-ttu-id="f490b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f490b-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="f490b-134">応答</span><span class="sxs-lookup"><span data-stu-id="f490b-134">Response</span></span>
<span data-ttu-id="f490b-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f490b-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
