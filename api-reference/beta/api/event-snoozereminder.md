---
title: 'イベント: snoozeReminder'
description: までは新しいユーザーの予定表にイベントのアラームを延期します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4197a231872341b7ba9c14057e32569b5c0f0c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966077"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="f4aed-103">イベント: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="f4aed-103">event: snoozeReminder</span></span>

> <span data-ttu-id="f4aed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4aed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4aed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4aed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4aed-106">までは新しいユーザー[の予定表](../resources/calendar.md)に[イベント](../resources/event.md)のアラームを延期します。</span><span class="sxs-lookup"><span data-stu-id="f4aed-106">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4aed-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4aed-107">Permissions</span></span>
<span data-ttu-id="f4aed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4aed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4aed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4aed-110">Permission type</span></span>      | <span data-ttu-id="f4aed-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4aed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4aed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4aed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4aed-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4aed-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f4aed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4aed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4aed-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4aed-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f4aed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4aed-116">Application</span></span> | <span data-ttu-id="f4aed-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4aed-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4aed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4aed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="f4aed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4aed-119">Request headers</span></span>
| <span data-ttu-id="f4aed-120">名前</span><span class="sxs-lookup"><span data-stu-id="f4aed-120">Name</span></span>       | <span data-ttu-id="f4aed-121">種類</span><span class="sxs-lookup"><span data-stu-id="f4aed-121">Type</span></span> | <span data-ttu-id="f4aed-122">説明</span><span class="sxs-lookup"><span data-stu-id="f4aed-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4aed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4aed-123">Authorization</span></span>  | <span data-ttu-id="f4aed-124">string</span><span class="sxs-lookup"><span data-stu-id="f4aed-124">string</span></span>  | <span data-ttu-id="f4aed-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f4aed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4aed-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4aed-127">Content-Type</span></span> | <span data-ttu-id="f4aed-128">string</span><span class="sxs-lookup"><span data-stu-id="f4aed-128">string</span></span>  | <span data-ttu-id="f4aed-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="f4aed-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4aed-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4aed-131">Request body</span></span>
<span data-ttu-id="f4aed-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f4aed-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4aed-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4aed-133">Parameter</span></span>    | <span data-ttu-id="f4aed-134">Type</span><span class="sxs-lookup"><span data-stu-id="f4aed-134">Type</span></span>   |<span data-ttu-id="f4aed-135">説明</span><span class="sxs-lookup"><span data-stu-id="f4aed-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4aed-136">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="f4aed-136">newReminderTime</span></span>|<span data-ttu-id="f4aed-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4aed-137">DateTimeTimeZone</span></span>|<span data-ttu-id="f4aed-138">アラームをトリガーする新しい日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f4aed-138">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="f4aed-139">応答</span><span class="sxs-lookup"><span data-stu-id="f4aed-139">Response</span></span>

<span data-ttu-id="f4aed-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f4aed-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4aed-142">例</span><span class="sxs-lookup"><span data-stu-id="f4aed-142">Example</span></span>
<span data-ttu-id="f4aed-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f4aed-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4aed-144">要求</span><span class="sxs-lookup"><span data-stu-id="f4aed-144">Request</span></span>
<span data-ttu-id="f4aed-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4aed-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "2016-10-19T10:37:00Z",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="f4aed-146">応答</span><span class="sxs-lookup"><span data-stu-id="f4aed-146">Response</span></span>
<span data-ttu-id="f4aed-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f4aed-147">Here is an example of the response.</span></span>
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
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
