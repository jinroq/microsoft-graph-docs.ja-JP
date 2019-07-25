---
title: 'イベント: 転送'
description: 'このアクションにより、会議イベントの開催者または出席者が '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 391263a5f2e9b5de2256830b986c9582b6299af2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859652"
---
# <a name="event-forward"></a><span data-ttu-id="03be5-103">イベント: 転送</span><span class="sxs-lookup"><span data-stu-id="03be5-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03be5-104">このアクションにより、会議[イベント](../resources/event.md)の開催者または出席者は、新しい受信者に会議出席依頼を転送することができます。</span><span class="sxs-lookup"><span data-stu-id="03be5-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="03be5-105">会議イベントが出席者の Office 365 メールボックスから別の受信者に転送された場合、この操作を行うと、転送先を開催者に通知するメッセージも送信され、受信者は会議イベントの開催者のコピーに追加されます。</span><span class="sxs-lookup"><span data-stu-id="03be5-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="03be5-106">この利便性は、Outlook.com アカウントから転送する場合には使用できません。</span><span class="sxs-lookup"><span data-stu-id="03be5-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="03be5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03be5-107">Permissions</span></span>
<span data-ttu-id="03be5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03be5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03be5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03be5-110">Permission type</span></span>      | <span data-ttu-id="03be5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03be5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03be5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03be5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03be5-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03be5-113">Calendars.Read</span></span>    |
|<span data-ttu-id="03be5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03be5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03be5-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03be5-115">Calendars.Read</span></span>    |
|<span data-ttu-id="03be5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03be5-116">Application</span></span> | <span data-ttu-id="03be5-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="03be5-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="03be5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03be5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/forward
POST /users/{id | userPrincipalName}/events/{id}/forward
POST /groups/{id}/events/{id}/forward

POST /me/calendar/events/{id}/forward
POST /users/{id | userPrincipalName}/calendar/events/{id}/forward
POST /groups/{id}/calendar/events/{id}/forward

POST /me/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/forward

POST /me/calendargroup/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/forward

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="03be5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03be5-119">Request headers</span></span>
| <span data-ttu-id="03be5-120">名前</span><span class="sxs-lookup"><span data-stu-id="03be5-120">Name</span></span>       | <span data-ttu-id="03be5-121">型</span><span class="sxs-lookup"><span data-stu-id="03be5-121">Type</span></span> | <span data-ttu-id="03be5-122">説明</span><span class="sxs-lookup"><span data-stu-id="03be5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03be5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03be5-123">Authorization</span></span>  | <span data-ttu-id="03be5-124">string</span><span class="sxs-lookup"><span data-stu-id="03be5-124">string</span></span>  | <span data-ttu-id="03be5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03be5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03be5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03be5-127">Content-Type</span></span> | <span data-ttu-id="03be5-128">string</span><span class="sxs-lookup"><span data-stu-id="03be5-128">string</span></span>  | <span data-ttu-id="03be5-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="03be5-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03be5-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="03be5-131">Request body</span></span>
<span data-ttu-id="03be5-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="03be5-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03be5-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="03be5-133">Parameter</span></span>    | <span data-ttu-id="03be5-134">型</span><span class="sxs-lookup"><span data-stu-id="03be5-134">Type</span></span>   |<span data-ttu-id="03be5-135">説明</span><span class="sxs-lookup"><span data-stu-id="03be5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03be5-136">Comment</span><span class="sxs-lookup"><span data-stu-id="03be5-136">Comment</span></span>|<span data-ttu-id="03be5-137">String</span><span class="sxs-lookup"><span data-stu-id="03be5-137">String</span></span>|<span data-ttu-id="03be5-p105">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="03be5-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="03be5-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="03be5-140">ToRecipients</span></span>|<span data-ttu-id="03be5-141">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="03be5-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="03be5-142">イベントを転送する受信者の一覧。</span><span class="sxs-lookup"><span data-stu-id="03be5-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="03be5-143">応答</span><span class="sxs-lookup"><span data-stu-id="03be5-143">Response</span></span>

<span data-ttu-id="03be5-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="03be5-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03be5-146">例</span><span class="sxs-lookup"><span data-stu-id="03be5-146">Example</span></span>
<span data-ttu-id="03be5-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="03be5-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03be5-148">要求</span><span class="sxs-lookup"><span data-stu-id="03be5-148">Request</span></span>
<span data-ttu-id="03be5-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03be5-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03be5-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="03be5-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/forward
Content-type: application/json
Content-length: 56

{
  "ToRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ],
  "Comment": "Dana, hope you can make this meeting." 
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03be5-151">C#</span><span class="sxs-lookup"><span data-stu-id="03be5-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03be5-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="03be5-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03be5-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="03be5-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="03be5-154">Java</span><span class="sxs-lookup"><span data-stu-id="03be5-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="03be5-155">応答</span><span class="sxs-lookup"><span data-stu-id="03be5-155">Response</span></span>
<span data-ttu-id="03be5-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="03be5-156">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
