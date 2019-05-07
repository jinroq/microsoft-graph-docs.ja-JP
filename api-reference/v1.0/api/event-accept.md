---
title: 'イベント: 承諾'
description: ユーザーの予定表の指定のイベントを承諾します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0c75f000021e18f2d8b76cb99c7dfc308a7310ee
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615589"
---
# <a name="event-accept"></a><span data-ttu-id="fe56e-103">イベント: 承諾</span><span class="sxs-lookup"><span data-stu-id="fe56e-103">event: accept</span></span>

<span data-ttu-id="fe56e-104">ユーザーの[予定表](../resources/calendar.md)で指定した[イベント](../resources/event.md)を承諾します。</span><span class="sxs-lookup"><span data-stu-id="fe56e-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe56e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe56e-105">Permissions</span></span>
<span data-ttu-id="fe56e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe56e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe56e-108">Permission type</span></span>      | <span data-ttu-id="fe56e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe56e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe56e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe56e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe56e-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe56e-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fe56e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe56e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe56e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe56e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fe56e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe56e-114">Application</span></span> | <span data-ttu-id="fe56e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe56e-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe56e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe56e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="fe56e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe56e-117">Request headers</span></span>
| <span data-ttu-id="fe56e-118">名前</span><span class="sxs-lookup"><span data-stu-id="fe56e-118">Name</span></span>       | <span data-ttu-id="fe56e-119">型</span><span class="sxs-lookup"><span data-stu-id="fe56e-119">Type</span></span> | <span data-ttu-id="fe56e-120">説明</span><span class="sxs-lookup"><span data-stu-id="fe56e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe56e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe56e-121">Authorization</span></span>  | <span data-ttu-id="fe56e-122">string</span><span class="sxs-lookup"><span data-stu-id="fe56e-122">string</span></span>  | <span data-ttu-id="fe56e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe56e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe56e-125">Content-Type</span></span> | <span data-ttu-id="fe56e-126">string</span><span class="sxs-lookup"><span data-stu-id="fe56e-126">string</span></span>  | <span data-ttu-id="fe56e-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe56e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe56e-129">Request body</span></span>
<span data-ttu-id="fe56e-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fe56e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe56e-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe56e-131">Parameter</span></span>    | <span data-ttu-id="fe56e-132">型</span><span class="sxs-lookup"><span data-stu-id="fe56e-132">Type</span></span>   |<span data-ttu-id="fe56e-133">説明</span><span class="sxs-lookup"><span data-stu-id="fe56e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe56e-134">comment</span><span class="sxs-lookup"><span data-stu-id="fe56e-134">comment</span></span>|<span data-ttu-id="fe56e-135">String</span><span class="sxs-lookup"><span data-stu-id="fe56e-135">String</span></span>|<span data-ttu-id="fe56e-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="fe56e-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="fe56e-138">sendResponse</span></span>|<span data-ttu-id="fe56e-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe56e-139">Boolean</span></span>|<span data-ttu-id="fe56e-p105">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="fe56e-143">応答</span><span class="sxs-lookup"><span data-stu-id="fe56e-143">Response</span></span>

<span data-ttu-id="fe56e-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fe56e-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe56e-146">例</span><span class="sxs-lookup"><span data-stu-id="fe56e-146">Example</span></span>
<span data-ttu-id="fe56e-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fe56e-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe56e-148">要求</span><span class="sxs-lookup"><span data-stu-id="fe56e-148">Request</span></span>
<span data-ttu-id="fe56e-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe56e-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="fe56e-150">応答</span><span class="sxs-lookup"><span data-stu-id="fe56e-150">Response</span></span>
<span data-ttu-id="fe56e-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="fe56e-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe56e-152">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="fe56e-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe56e-153">Visual</span><span class="sxs-lookup"><span data-stu-id="fe56e-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_accept-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe56e-154">Java</span><span class="sxs-lookup"><span data-stu-id="fe56e-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_accept-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-accept.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
