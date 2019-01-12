---
title: 'イベント: 転送'
description: 'この操作により、開催者または転送するように会議のイベントの参加者、 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fe8d108ebeb15c2684e1997b8a02cc28a99101b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990674"
---
# <a name="event-forward"></a><span data-ttu-id="c9889-103">イベント: 転送</span><span class="sxs-lookup"><span data-stu-id="c9889-103">event: forward</span></span>

> <span data-ttu-id="c9889-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9889-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9889-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9889-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9889-106">このアクションでは、開催者または新しい受信者に会議出席依頼を転送する[イベント](../resources/event.md)の会議の出席者を使用します。</span><span class="sxs-lookup"><span data-stu-id="c9889-106">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="c9889-107">会議イベントは、出席者の Office 365 のメールボックスから別の受信者に転送されます、このアクションも、転送の構成内容の変更を通知するためにメッセージを送信し、会議イベントの開催者のコピーに受信者を追加します。</span><span class="sxs-lookup"><span data-stu-id="c9889-107">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="c9889-108">Outlook.com アカウントから転送するときは、この利便性を利用できません。</span><span class="sxs-lookup"><span data-stu-id="c9889-108">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="c9889-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c9889-109">Permissions</span></span>
<span data-ttu-id="c9889-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9889-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9889-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9889-112">Permission type</span></span>      | <span data-ttu-id="c9889-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9889-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9889-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9889-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c9889-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c9889-115">Calendars.Read</span></span>    |
|<span data-ttu-id="c9889-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9889-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9889-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c9889-117">Calendars.Read</span></span>    |
|<span data-ttu-id="c9889-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9889-118">Application</span></span> | <span data-ttu-id="c9889-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c9889-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9889-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9889-120">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="c9889-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9889-121">Request headers</span></span>
| <span data-ttu-id="c9889-122">名前</span><span class="sxs-lookup"><span data-stu-id="c9889-122">Name</span></span>       | <span data-ttu-id="c9889-123">型</span><span class="sxs-lookup"><span data-stu-id="c9889-123">Type</span></span> | <span data-ttu-id="c9889-124">説明</span><span class="sxs-lookup"><span data-stu-id="c9889-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9889-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9889-125">Authorization</span></span>  | <span data-ttu-id="c9889-126">string</span><span class="sxs-lookup"><span data-stu-id="c9889-126">string</span></span>  | <span data-ttu-id="c9889-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c9889-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9889-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9889-129">Content-Type</span></span> | <span data-ttu-id="c9889-130">string</span><span class="sxs-lookup"><span data-stu-id="c9889-130">string</span></span>  | <span data-ttu-id="c9889-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="c9889-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9889-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9889-133">Request body</span></span>
<span data-ttu-id="c9889-134">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9889-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9889-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9889-135">Parameter</span></span>    | <span data-ttu-id="c9889-136">型</span><span class="sxs-lookup"><span data-stu-id="c9889-136">Type</span></span>   |<span data-ttu-id="c9889-137">説明</span><span class="sxs-lookup"><span data-stu-id="c9889-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9889-138">Comment</span><span class="sxs-lookup"><span data-stu-id="c9889-138">Comment</span></span>|<span data-ttu-id="c9889-139">String</span><span class="sxs-lookup"><span data-stu-id="c9889-139">String</span></span>|<span data-ttu-id="c9889-p106">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c9889-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="c9889-142">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="c9889-142">ToRecipients</span></span>|<span data-ttu-id="c9889-143">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="c9889-143">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c9889-144">イベントを転送する受信者の一覧。</span><span class="sxs-lookup"><span data-stu-id="c9889-144">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="c9889-145">応答</span><span class="sxs-lookup"><span data-stu-id="c9889-145">Response</span></span>

<span data-ttu-id="c9889-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c9889-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9889-148">例</span><span class="sxs-lookup"><span data-stu-id="c9889-148">Example</span></span>
<span data-ttu-id="c9889-149">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c9889-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9889-150">要求</span><span class="sxs-lookup"><span data-stu-id="c9889-150">Request</span></span>
<span data-ttu-id="c9889-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9889-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c9889-152">応答</span><span class="sxs-lookup"><span data-stu-id="c9889-152">Response</span></span>
<span data-ttu-id="c9889-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c9889-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
