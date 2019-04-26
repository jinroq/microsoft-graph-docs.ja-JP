---
title: 'イベント: 承諾'
description: ユーザーの予定表の指定のイベントを承諾します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2a137d59a4df8c3e02121de74c4158978ad397a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324930"
---
# <a name="event-accept"></a><span data-ttu-id="85f3a-103">イベント: 承諾</span><span class="sxs-lookup"><span data-stu-id="85f3a-103">event: accept</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f3a-104">ユーザーの[予定表](../resources/calendar.md)で指定した[イベント](../resources/event.md)を承諾します。</span><span class="sxs-lookup"><span data-stu-id="85f3a-104">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85f3a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85f3a-105">Permissions</span></span>
<span data-ttu-id="85f3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f3a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85f3a-108">Permission type</span></span>      | <span data-ttu-id="85f3a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85f3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85f3a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85f3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85f3a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85f3a-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="85f3a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85f3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85f3a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85f3a-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="85f3a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85f3a-114">Application</span></span> | <span data-ttu-id="85f3a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85f3a-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85f3a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85f3a-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="85f3a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85f3a-117">Request headers</span></span>
| <span data-ttu-id="85f3a-118">名前</span><span class="sxs-lookup"><span data-stu-id="85f3a-118">Name</span></span>       | <span data-ttu-id="85f3a-119">型</span><span class="sxs-lookup"><span data-stu-id="85f3a-119">Type</span></span> | <span data-ttu-id="85f3a-120">説明</span><span class="sxs-lookup"><span data-stu-id="85f3a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85f3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f3a-121">Authorization</span></span>  | <span data-ttu-id="85f3a-122">string</span><span class="sxs-lookup"><span data-stu-id="85f3a-122">string</span></span>  | <span data-ttu-id="85f3a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85f3a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85f3a-125">Content-Type</span></span> | <span data-ttu-id="85f3a-126">string</span><span class="sxs-lookup"><span data-stu-id="85f3a-126">string</span></span>  | <span data-ttu-id="85f3a-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85f3a-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="85f3a-129">Request body</span></span>
<span data-ttu-id="85f3a-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="85f3a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="85f3a-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="85f3a-131">Parameter</span></span>    | <span data-ttu-id="85f3a-132">型</span><span class="sxs-lookup"><span data-stu-id="85f3a-132">Type</span></span>   |<span data-ttu-id="85f3a-133">説明</span><span class="sxs-lookup"><span data-stu-id="85f3a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85f3a-134">comment</span><span class="sxs-lookup"><span data-stu-id="85f3a-134">comment</span></span>|<span data-ttu-id="85f3a-135">String</span><span class="sxs-lookup"><span data-stu-id="85f3a-135">String</span></span>|<span data-ttu-id="85f3a-p104">応答に含まれるテキスト。省略可。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="85f3a-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="85f3a-138">sendResponse</span></span>|<span data-ttu-id="85f3a-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="85f3a-139">Boolean</span></span>|<span data-ttu-id="85f3a-p105">応答が開催者に送信される場合は、`true`。それ以外の場合は、`false`。省略可。既定値は `true` です。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="85f3a-143">応答</span><span class="sxs-lookup"><span data-stu-id="85f3a-143">Response</span></span>

<span data-ttu-id="85f3a-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="85f3a-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f3a-146">例</span><span class="sxs-lookup"><span data-stu-id="85f3a-146">Example</span></span>
<span data-ttu-id="85f3a-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="85f3a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85f3a-148">要求</span><span class="sxs-lookup"><span data-stu-id="85f3a-148">Request</span></span>
<span data-ttu-id="85f3a-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85f3a-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="85f3a-150">応答</span><span class="sxs-lookup"><span data-stu-id="85f3a-150">Response</span></span>
<span data-ttu-id="85f3a-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="85f3a-151">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
