---
title: 'イベント: tentativelyAccept'
description: ユーザーの予定表の指定のイベントを仮承諾します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ce5f4012ded4c4c63a8c4b4fec8f997eb970cf97
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859456"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="bae66-103">イベント: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="bae66-103">event: tentativelyAccept</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bae66-104">ユーザーの[予定表](../resources/calendar.md)で指定した[イベント](../resources/event.md)を仮承諾します。</span><span class="sxs-lookup"><span data-stu-id="bae66-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bae66-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bae66-105">Permissions</span></span>
<span data-ttu-id="bae66-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bae66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae66-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bae66-108">Permission type</span></span>      | <span data-ttu-id="bae66-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bae66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bae66-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bae66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bae66-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae66-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bae66-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bae66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae66-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae66-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bae66-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bae66-114">Application</span></span> | <span data-ttu-id="bae66-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bae66-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bae66-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bae66-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="bae66-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bae66-117">Request headers</span></span>
| <span data-ttu-id="bae66-118">名前</span><span class="sxs-lookup"><span data-stu-id="bae66-118">Name</span></span>       | <span data-ttu-id="bae66-119">型</span><span class="sxs-lookup"><span data-stu-id="bae66-119">Type</span></span> | <span data-ttu-id="bae66-120">説明</span><span class="sxs-lookup"><span data-stu-id="bae66-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bae66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae66-121">Authorization</span></span>  | <span data-ttu-id="bae66-122">string</span><span class="sxs-lookup"><span data-stu-id="bae66-122">string</span></span>  | <span data-ttu-id="bae66-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bae66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bae66-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bae66-125">Content-Type</span></span> | <span data-ttu-id="bae66-126">string</span><span class="sxs-lookup"><span data-stu-id="bae66-126">string</span></span>  | <span data-ttu-id="bae66-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="bae66-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bae66-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bae66-129">Request body</span></span>
<span data-ttu-id="bae66-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bae66-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bae66-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bae66-131">Parameter</span></span>    | <span data-ttu-id="bae66-132">型</span><span class="sxs-lookup"><span data-stu-id="bae66-132">Type</span></span>   |<span data-ttu-id="bae66-133">説明</span><span class="sxs-lookup"><span data-stu-id="bae66-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bae66-134">comment</span><span class="sxs-lookup"><span data-stu-id="bae66-134">comment</span></span>|<span data-ttu-id="bae66-135">String</span><span class="sxs-lookup"><span data-stu-id="bae66-135">String</span></span>|<span data-ttu-id="bae66-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="bae66-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="bae66-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="bae66-138">sendResponse</span></span>|<span data-ttu-id="bae66-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="bae66-139">Boolean</span></span>|<span data-ttu-id="bae66-p105">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="bae66-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="bae66-143">応答</span><span class="sxs-lookup"><span data-stu-id="bae66-143">Response</span></span>

<span data-ttu-id="bae66-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bae66-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae66-146">例</span><span class="sxs-lookup"><span data-stu-id="bae66-146">Example</span></span>
<span data-ttu-id="bae66-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bae66-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bae66-148">要求</span><span class="sxs-lookup"><span data-stu-id="bae66-148">Request</span></span>
<span data-ttu-id="bae66-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bae66-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bae66-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="bae66-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bae66-151">C#</span><span class="sxs-lookup"><span data-stu-id="bae66-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bae66-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="bae66-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bae66-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="bae66-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bae66-154">Java</span><span class="sxs-lookup"><span data-stu-id="bae66-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bae66-155">応答</span><span class="sxs-lookup"><span data-stu-id="bae66-155">Response</span></span>
##### <a name="response"></a><span data-ttu-id="bae66-156">応答</span><span class="sxs-lookup"><span data-stu-id="bae66-156">Response</span></span>
<span data-ttu-id="bae66-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bae66-157">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
