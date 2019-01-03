---
title: 'イベント: キャンセル'
description: 'このアクションにより、会議の開催者はキャンセル メッセージを送信し、イベントをキャンセルできます。 '
author: angelgolfer-ms
ms.openlocfilehash: 5e32219be129d1b16e05badd1fb778f86d95849b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350310"
---
# <a name="event-cancel"></a><span data-ttu-id="d9eaa-103">イベント: キャンセル</span><span class="sxs-lookup"><span data-stu-id="d9eaa-103">event: cancel</span></span>

> <span data-ttu-id="d9eaa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9eaa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9eaa-106">このアクションにより、会議の開催者はキャンセル メッセージを送信し、イベントをキャンセルできます。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-106">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="d9eaa-p102">アクションは、イベントを削除済みアイテム フォルダーに移動します。開催者は、発生イベント ID を指定することで、定期的な会議の開催をキャンセルすることもできます。この操作を呼び出す出席者には、エラー (HTTP 400: 要求が正しくありません) が次のエラー メッセージと共に通知されます。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p102">The action moves the event to the Deleted Items folder. The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID. An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="d9eaa-p103">"要求を完了できません。会議を取り消すには、開催者である必要があります。"</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p103">"Your request can't be completed. You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="d9eaa-112">このアクションは、開催者に対してのみ**キャンセル**が使用可能であるという点で、[削除](event-delete.md)とは異なり、開催者はキャンセルに関するカスタム メッセージを出席者に送信できます。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-112">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9eaa-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d9eaa-113">Permissions</span></span>
<span data-ttu-id="d9eaa-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9eaa-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d9eaa-116">Permission type</span></span>      | <span data-ttu-id="d9eaa-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d9eaa-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9eaa-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d9eaa-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d9eaa-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9eaa-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d9eaa-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d9eaa-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9eaa-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9eaa-121">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d9eaa-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d9eaa-122">Application</span></span> | <span data-ttu-id="d9eaa-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9eaa-123">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9eaa-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d9eaa-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="d9eaa-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d9eaa-125">Request headers</span></span>
| <span data-ttu-id="d9eaa-126">名前</span><span class="sxs-lookup"><span data-stu-id="d9eaa-126">Name</span></span>       | <span data-ttu-id="d9eaa-127">種類</span><span class="sxs-lookup"><span data-stu-id="d9eaa-127">Type</span></span> | <span data-ttu-id="d9eaa-128">説明</span><span class="sxs-lookup"><span data-stu-id="d9eaa-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9eaa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9eaa-129">Authorization</span></span>  | <span data-ttu-id="d9eaa-130">string</span><span class="sxs-lookup"><span data-stu-id="d9eaa-130">string</span></span>  | <span data-ttu-id="d9eaa-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9eaa-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9eaa-133">Content-Type</span></span> | <span data-ttu-id="d9eaa-134">string</span><span class="sxs-lookup"><span data-stu-id="d9eaa-134">string</span></span>  | <span data-ttu-id="d9eaa-p106">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9eaa-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="d9eaa-137">Request body</span></span>
<span data-ttu-id="d9eaa-138">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d9eaa-139">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d9eaa-139">Parameter</span></span>    | <span data-ttu-id="d9eaa-140">種類</span><span class="sxs-lookup"><span data-stu-id="d9eaa-140">Type</span></span>   |<span data-ttu-id="d9eaa-141">説明</span><span class="sxs-lookup"><span data-stu-id="d9eaa-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9eaa-142">comment</span><span class="sxs-lookup"><span data-stu-id="d9eaa-142">comment</span></span>|<span data-ttu-id="d9eaa-143">String</span><span class="sxs-lookup"><span data-stu-id="d9eaa-143">String</span></span>|<span data-ttu-id="d9eaa-144">すべての出席者に送信されるキャンセルに関するコメント。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-144">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="d9eaa-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-145">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="d9eaa-146">応答</span><span class="sxs-lookup"><span data-stu-id="d9eaa-146">Response</span></span>

<span data-ttu-id="d9eaa-p108">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9eaa-149">例</span><span class="sxs-lookup"><span data-stu-id="d9eaa-149">Example</span></span>
<span data-ttu-id="d9eaa-150">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9eaa-151">要求</span><span class="sxs-lookup"><span data-stu-id="d9eaa-151">Request</span></span>
<span data-ttu-id="d9eaa-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```

##### <a name="response"></a><span data-ttu-id="d9eaa-153">応答</span><span class="sxs-lookup"><span data-stu-id="d9eaa-153">Response</span></span>
<span data-ttu-id="d9eaa-154">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d9eaa-154">Here is an example of the response.</span></span>
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->