---
title: 'イベント: 辞退'
description: ユーザーの予定表で指定したイベントへの招待を辞退します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b59d6717d51dc2f72e49c8e4f971f54950674bc6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916501"
---
# <a name="event-decline"></a><span data-ttu-id="2b667-103">イベント: 辞退</span><span class="sxs-lookup"><span data-stu-id="2b667-103">event: decline</span></span>

> <span data-ttu-id="2b667-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b667-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b667-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b667-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b667-106">ユーザー[の予定表](../resources/calendar.md)で指定した[イベント](../resources/event.md)への招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="2b667-106">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b667-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b667-107">Permissions</span></span>
<span data-ttu-id="2b667-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b667-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b667-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b667-110">Permission type</span></span>      | <span data-ttu-id="2b667-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b667-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b667-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b667-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b667-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b667-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b667-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b667-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b667-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b667-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b667-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b667-116">Application</span></span> | <span data-ttu-id="2b667-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b667-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b667-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b667-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="2b667-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b667-119">Request headers</span></span>

| <span data-ttu-id="2b667-120">名前</span><span class="sxs-lookup"><span data-stu-id="2b667-120">Name</span></span>       | <span data-ttu-id="2b667-121">型</span><span class="sxs-lookup"><span data-stu-id="2b667-121">Type</span></span> | <span data-ttu-id="2b667-122">説明</span><span class="sxs-lookup"><span data-stu-id="2b667-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b667-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b667-123">Authorization</span></span>  | <span data-ttu-id="2b667-124">string</span><span class="sxs-lookup"><span data-stu-id="2b667-124">string</span></span>  | <span data-ttu-id="2b667-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b667-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b667-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b667-127">Content-Type</span></span> | <span data-ttu-id="2b667-128">string</span><span class="sxs-lookup"><span data-stu-id="2b667-128">string</span></span>  | <span data-ttu-id="2b667-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="2b667-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b667-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b667-131">Request body</span></span>

<span data-ttu-id="2b667-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b667-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b667-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b667-133">Parameter</span></span>    | <span data-ttu-id="2b667-134">型</span><span class="sxs-lookup"><span data-stu-id="2b667-134">Type</span></span>   |<span data-ttu-id="2b667-135">説明</span><span class="sxs-lookup"><span data-stu-id="2b667-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b667-136">comment</span><span class="sxs-lookup"><span data-stu-id="2b667-136">comment</span></span>|<span data-ttu-id="2b667-137">String</span><span class="sxs-lookup"><span data-stu-id="2b667-137">String</span></span>|<span data-ttu-id="2b667-p105">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="2b667-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2b667-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2b667-140">sendResponse</span></span>|<span data-ttu-id="2b667-141">ブール型</span><span class="sxs-lookup"><span data-stu-id="2b667-141">Boolean</span></span>|<span data-ttu-id="2b667-p106">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="2b667-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2b667-145">応答</span><span class="sxs-lookup"><span data-stu-id="2b667-145">Response</span></span>

<span data-ttu-id="2b667-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2b667-p107">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b667-148">例</span><span class="sxs-lookup"><span data-stu-id="2b667-148">Example</span></span>

<span data-ttu-id="2b667-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2b667-149">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2b667-150">要求</span><span class="sxs-lookup"><span data-stu-id="2b667-150">Request</span></span>

<span data-ttu-id="2b667-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b667-151">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

### <a name="response"></a><span data-ttu-id="2b667-152">応答</span><span class="sxs-lookup"><span data-stu-id="2b667-152">Response</span></span>

<span data-ttu-id="2b667-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2b667-153">Here is an example of the response.</span></span>

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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
