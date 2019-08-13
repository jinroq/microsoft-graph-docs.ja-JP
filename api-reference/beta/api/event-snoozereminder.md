---
title: 'イベント: snoozeReminder'
description: ユーザーの予定表にあるイベントのアラームを、新しい時刻まで延期します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f9c78dadf355af3da800e954da3b42f3dcc94260
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326878"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="81293-103">イベント: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="81293-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81293-104">ユーザーの[予定表](../resources/calendar.md)にある[イベント](../resources/event.md)のアラームを、新しい時刻まで延期します。</span><span class="sxs-lookup"><span data-stu-id="81293-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="81293-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="81293-105">Permissions</span></span>
<span data-ttu-id="81293-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81293-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81293-108">Permission type</span></span>      | <span data-ttu-id="81293-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="81293-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81293-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81293-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81293-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81293-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="81293-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81293-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81293-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81293-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="81293-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81293-114">Application</span></span> | <span data-ttu-id="81293-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81293-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="81293-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81293-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="81293-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81293-117">Request headers</span></span>
| <span data-ttu-id="81293-118">名前</span><span class="sxs-lookup"><span data-stu-id="81293-118">Name</span></span>       | <span data-ttu-id="81293-119">型</span><span class="sxs-lookup"><span data-stu-id="81293-119">Type</span></span> | <span data-ttu-id="81293-120">説明</span><span class="sxs-lookup"><span data-stu-id="81293-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81293-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81293-121">Authorization</span></span>  | <span data-ttu-id="81293-122">string</span><span class="sxs-lookup"><span data-stu-id="81293-122">string</span></span>  | <span data-ttu-id="81293-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="81293-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81293-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81293-125">Content-Type</span></span> | <span data-ttu-id="81293-126">string</span><span class="sxs-lookup"><span data-stu-id="81293-126">string</span></span>  | <span data-ttu-id="81293-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="81293-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81293-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="81293-129">Request body</span></span>
<span data-ttu-id="81293-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="81293-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81293-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="81293-131">Parameter</span></span>    | <span data-ttu-id="81293-132">型</span><span class="sxs-lookup"><span data-stu-id="81293-132">Type</span></span>   |<span data-ttu-id="81293-133">説明</span><span class="sxs-lookup"><span data-stu-id="81293-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81293-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="81293-134">newReminderTime</span></span>|<span data-ttu-id="81293-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="81293-135">DateTimeTimeZone</span></span>|<span data-ttu-id="81293-136">アラームをトリガーする新しい日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="81293-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="81293-137">応答</span><span class="sxs-lookup"><span data-stu-id="81293-137">Response</span></span>

<span data-ttu-id="81293-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="81293-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81293-140">例</span><span class="sxs-lookup"><span data-stu-id="81293-140">Example</span></span>
<span data-ttu-id="81293-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="81293-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81293-142">要求</span><span class="sxs-lookup"><span data-stu-id="81293-142">Request</span></span>
<span data-ttu-id="81293-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81293-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81293-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="81293-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="81293-145">C#</span><span class="sxs-lookup"><span data-stu-id="81293-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81293-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81293-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81293-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="81293-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81293-148">Java</span><span class="sxs-lookup"><span data-stu-id="81293-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-snoozereminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81293-149">応答</span><span class="sxs-lookup"><span data-stu-id="81293-149">Response</span></span>
<span data-ttu-id="81293-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="81293-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
