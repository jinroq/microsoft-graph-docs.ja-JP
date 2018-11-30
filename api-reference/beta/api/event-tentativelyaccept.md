---
title: 'イベント: tentativelyAccept'
description: ユーザーの予定表で指定したイベントを仮承諾します。
ms.openlocfilehash: 7e90f428f06c4bfaaaff063e38c9f159777a1e22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066357"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="9122a-103">イベント: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="9122a-103">event: tentativelyAccept</span></span>

> <span data-ttu-id="9122a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9122a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9122a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9122a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9122a-106">ユーザー[の予定表](../resources/calendar.md)で指定した[イベント](../resources/event.md)を仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="9122a-106">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9122a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9122a-107">Permissions</span></span>
<span data-ttu-id="9122a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9122a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9122a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9122a-110">Permission type</span></span>      | <span data-ttu-id="9122a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9122a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9122a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9122a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9122a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9122a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9122a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9122a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122a-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9122a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9122a-116">Application</span></span> | <span data-ttu-id="9122a-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122a-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9122a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9122a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="9122a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9122a-119">Request headers</span></span>
| <span data-ttu-id="9122a-120">名前</span><span class="sxs-lookup"><span data-stu-id="9122a-120">Name</span></span>       | <span data-ttu-id="9122a-121">型</span><span class="sxs-lookup"><span data-stu-id="9122a-121">Type</span></span> | <span data-ttu-id="9122a-122">説明</span><span class="sxs-lookup"><span data-stu-id="9122a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9122a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9122a-123">Authorization</span></span>  | <span data-ttu-id="9122a-124">string</span><span class="sxs-lookup"><span data-stu-id="9122a-124">string</span></span>  | <span data-ttu-id="9122a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9122a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9122a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9122a-127">Content-Type</span></span> | <span data-ttu-id="9122a-128">string</span><span class="sxs-lookup"><span data-stu-id="9122a-128">string</span></span>  | <span data-ttu-id="9122a-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="9122a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9122a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9122a-131">Request body</span></span>
<span data-ttu-id="9122a-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9122a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9122a-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9122a-133">Parameter</span></span>    | <span data-ttu-id="9122a-134">型</span><span class="sxs-lookup"><span data-stu-id="9122a-134">Type</span></span>   |<span data-ttu-id="9122a-135">説明</span><span class="sxs-lookup"><span data-stu-id="9122a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9122a-136">comment</span><span class="sxs-lookup"><span data-stu-id="9122a-136">comment</span></span>|<span data-ttu-id="9122a-137">String</span><span class="sxs-lookup"><span data-stu-id="9122a-137">String</span></span>|<span data-ttu-id="9122a-p105">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="9122a-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="9122a-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="9122a-140">sendResponse</span></span>|<span data-ttu-id="9122a-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="9122a-141">Boolean</span></span>|<span data-ttu-id="9122a-p106">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="9122a-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="9122a-145">応答</span><span class="sxs-lookup"><span data-stu-id="9122a-145">Response</span></span>

<span data-ttu-id="9122a-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9122a-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9122a-148">例</span><span class="sxs-lookup"><span data-stu-id="9122a-148">Example</span></span>
<span data-ttu-id="9122a-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9122a-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9122a-150">要求</span><span class="sxs-lookup"><span data-stu-id="9122a-150">Request</span></span>
<span data-ttu-id="9122a-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9122a-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="9122a-152">応答</span><span class="sxs-lookup"><span data-stu-id="9122a-152">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9122a-153">応答</span><span class="sxs-lookup"><span data-stu-id="9122a-153">Response</span></span>
<span data-ttu-id="9122a-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9122a-154">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
