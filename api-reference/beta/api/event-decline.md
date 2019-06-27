---
title: 'イベント: 辞退'
description: ユーザーの予定表の指定のイベントに対する詳細を辞退します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3b6f648d5bbe3adbff5fcfd4f852a2b1c5e75a79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259235"
---
# <a name="event-decline"></a><span data-ttu-id="dca8c-103">イベント: 辞退</span><span class="sxs-lookup"><span data-stu-id="dca8c-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca8c-104">ユーザーの[予定表](../resources/calendar.md)の指定した[イベント](../resources/event.md)への招待を辞退します。</span><span class="sxs-lookup"><span data-stu-id="dca8c-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dca8c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dca8c-105">Permissions</span></span>
<span data-ttu-id="dca8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca8c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dca8c-108">Permission type</span></span>      | <span data-ttu-id="dca8c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dca8c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dca8c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dca8c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dca8c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca8c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dca8c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dca8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca8c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca8c-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dca8c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dca8c-114">Application</span></span> | <span data-ttu-id="dca8c-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dca8c-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dca8c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dca8c-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="dca8c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dca8c-117">Request headers</span></span>

| <span data-ttu-id="dca8c-118">名前</span><span class="sxs-lookup"><span data-stu-id="dca8c-118">Name</span></span>       | <span data-ttu-id="dca8c-119">型</span><span class="sxs-lookup"><span data-stu-id="dca8c-119">Type</span></span> | <span data-ttu-id="dca8c-120">説明</span><span class="sxs-lookup"><span data-stu-id="dca8c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dca8c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dca8c-121">Authorization</span></span>  | <span data-ttu-id="dca8c-122">string</span><span class="sxs-lookup"><span data-stu-id="dca8c-122">string</span></span>  | <span data-ttu-id="dca8c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dca8c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dca8c-125">Content-Type</span></span> | <span data-ttu-id="dca8c-126">string</span><span class="sxs-lookup"><span data-stu-id="dca8c-126">string</span></span>  | <span data-ttu-id="dca8c-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dca8c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="dca8c-129">Request body</span></span>

<span data-ttu-id="dca8c-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dca8c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dca8c-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dca8c-131">Parameter</span></span>    | <span data-ttu-id="dca8c-132">型</span><span class="sxs-lookup"><span data-stu-id="dca8c-132">Type</span></span>   |<span data-ttu-id="dca8c-133">説明</span><span class="sxs-lookup"><span data-stu-id="dca8c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dca8c-134">comment</span><span class="sxs-lookup"><span data-stu-id="dca8c-134">comment</span></span>|<span data-ttu-id="dca8c-135">String</span><span class="sxs-lookup"><span data-stu-id="dca8c-135">String</span></span>|<span data-ttu-id="dca8c-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="dca8c-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="dca8c-138">sendResponse</span></span>|<span data-ttu-id="dca8c-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="dca8c-139">Boolean</span></span>|<span data-ttu-id="dca8c-p105">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="dca8c-143">応答</span><span class="sxs-lookup"><span data-stu-id="dca8c-143">Response</span></span>

<span data-ttu-id="dca8c-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dca8c-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca8c-146">例</span><span class="sxs-lookup"><span data-stu-id="dca8c-146">Example</span></span>

<span data-ttu-id="dca8c-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dca8c-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dca8c-148">要求</span><span class="sxs-lookup"><span data-stu-id="dca8c-148">Request</span></span>

<span data-ttu-id="dca8c-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dca8c-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="dca8c-150">応答</span><span class="sxs-lookup"><span data-stu-id="dca8c-150">Response</span></span>

<span data-ttu-id="dca8c-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dca8c-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dca8c-152">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="dca8c-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dca8c-153">C#</span><span class="sxs-lookup"><span data-stu-id="dca8c-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_decline-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dca8c-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="dca8c-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_decline-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dca8c-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="dca8c-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_decline-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
