---
title: 'イベント: snoozeReminder'
description: ユーザーの予定表にあるイベントのアラームを、新しい時刻まで延期します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 53643800e9148297be166e4f41deaa4eaf9ca542
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586681"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="ddc2f-103">イベント: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="ddc2f-103">event: snoozeReminder</span></span>

<span data-ttu-id="ddc2f-104">ユーザーの[予定表](../resources/calendar.md)にある[イベント](../resources/event.md)のアラームを、新しい時刻まで延期します。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddc2f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddc2f-105">Permissions</span></span>
<span data-ttu-id="ddc2f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc2f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ddc2f-108">Permission type</span></span>      | <span data-ttu-id="ddc2f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ddc2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddc2f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ddc2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ddc2f-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddc2f-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ddc2f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ddc2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc2f-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddc2f-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ddc2f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ddc2f-114">Application</span></span> | <span data-ttu-id="ddc2f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddc2f-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddc2f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ddc2f-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ddc2f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddc2f-117">Request headers</span></span>
| <span data-ttu-id="ddc2f-118">名前</span><span class="sxs-lookup"><span data-stu-id="ddc2f-118">Name</span></span>       | <span data-ttu-id="ddc2f-119">型</span><span class="sxs-lookup"><span data-stu-id="ddc2f-119">Type</span></span> | <span data-ttu-id="ddc2f-120">説明</span><span class="sxs-lookup"><span data-stu-id="ddc2f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ddc2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddc2f-121">Authorization</span></span>  | <span data-ttu-id="ddc2f-122">string</span><span class="sxs-lookup"><span data-stu-id="ddc2f-122">string</span></span>  | <span data-ttu-id="ddc2f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddc2f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddc2f-125">Content-Type</span></span> | <span data-ttu-id="ddc2f-126">string</span><span class="sxs-lookup"><span data-stu-id="ddc2f-126">string</span></span>  | <span data-ttu-id="ddc2f-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddc2f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ddc2f-129">Request body</span></span>
<span data-ttu-id="ddc2f-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddc2f-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ddc2f-131">Parameter</span></span>    | <span data-ttu-id="ddc2f-132">型</span><span class="sxs-lookup"><span data-stu-id="ddc2f-132">Type</span></span>   |<span data-ttu-id="ddc2f-133">説明</span><span class="sxs-lookup"><span data-stu-id="ddc2f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddc2f-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="ddc2f-134">newReminderTime</span></span>|<span data-ttu-id="ddc2f-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ddc2f-135">DateTimeTimeZone</span></span>|<span data-ttu-id="ddc2f-136">アラームをトリガーする新しい日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="ddc2f-137">応答</span><span class="sxs-lookup"><span data-stu-id="ddc2f-137">Response</span></span>

<span data-ttu-id="ddc2f-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddc2f-140">例</span><span class="sxs-lookup"><span data-stu-id="ddc2f-140">Example</span></span>
<span data-ttu-id="ddc2f-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ddc2f-142">要求</span><span class="sxs-lookup"><span data-stu-id="ddc2f-142">Request</span></span>
<span data-ttu-id="ddc2f-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="ddc2f-144">応答</span><span class="sxs-lookup"><span data-stu-id="ddc2f-144">Response</span></span>
<span data-ttu-id="ddc2f-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ddc2f-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ddc2f-146">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ddc2f-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ddc2f-147">Visual</span><span class="sxs-lookup"><span data-stu-id="ddc2f-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_snoozereminder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddc2f-148">Java</span><span class="sxs-lookup"><span data-stu-id="ddc2f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_snoozereminder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-snoozereminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-snoozereminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
