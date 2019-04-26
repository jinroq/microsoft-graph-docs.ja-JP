---
title: 'イベント: キャンセル'
description: 'このアクションでは、会議の開催者はキャンセル メッセージを送信し、イベントをキャンセルできます。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bce1c979ff72fb454cef380715aa5a3fe6aec9c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33321934"
---
# <a name="event-cancel"></a><span data-ttu-id="bfff1-103">イベント: キャンセル</span><span class="sxs-lookup"><span data-stu-id="bfff1-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfff1-104">このアクションでは、会議の開催者はキャンセル メッセージを送信し、イベントをキャンセルできます。</span><span class="sxs-lookup"><span data-stu-id="bfff1-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="bfff1-p101">アクションは、イベントを削除済みアイテム フォルダーに移動します。 開催者は、発生イベント ID を指定することで、定期的な会議の開催をキャンセルすることもできます。 この操作を呼び出す出席者には、エラー (HTTP 400: 要求が正しくありません) が次のエラー メッセージと共に通知されます。</span><span class="sxs-lookup"><span data-stu-id="bfff1-p101">The action moves the event to the Deleted Items folder. The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID. An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="bfff1-p102">"要求を完了できません。 会議を取り消すには、開催者である必要があります。"</span><span class="sxs-lookup"><span data-stu-id="bfff1-p102">"Your request can't be completed. You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="bfff1-110">このアクションは、開催者に対してのみ[キャンセル](event-delete.md)が使用可能であるという点で、**削除**とは異なり、開催者はキャンセルに関するカスタム メッセージを出席者に送信できます。</span><span class="sxs-lookup"><span data-stu-id="bfff1-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfff1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bfff1-111">Permissions</span></span>
<span data-ttu-id="bfff1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfff1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfff1-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bfff1-114">Permission type</span></span>      | <span data-ttu-id="bfff1-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bfff1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfff1-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bfff1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bfff1-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfff1-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bfff1-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bfff1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfff1-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfff1-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bfff1-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bfff1-120">Application</span></span> | <span data-ttu-id="bfff1-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfff1-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfff1-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bfff1-122">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="bfff1-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfff1-123">Request headers</span></span>
| <span data-ttu-id="bfff1-124">名前</span><span class="sxs-lookup"><span data-stu-id="bfff1-124">Name</span></span>       | <span data-ttu-id="bfff1-125">型</span><span class="sxs-lookup"><span data-stu-id="bfff1-125">Type</span></span> | <span data-ttu-id="bfff1-126">説明</span><span class="sxs-lookup"><span data-stu-id="bfff1-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfff1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfff1-127">Authorization</span></span>  | <span data-ttu-id="bfff1-128">string</span><span class="sxs-lookup"><span data-stu-id="bfff1-128">string</span></span>  | <span data-ttu-id="bfff1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bfff1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfff1-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfff1-131">Content-Type</span></span> | <span data-ttu-id="bfff1-132">string</span><span class="sxs-lookup"><span data-stu-id="bfff1-132">string</span></span>  | <span data-ttu-id="bfff1-p105">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="bfff1-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfff1-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="bfff1-135">Request body</span></span>
<span data-ttu-id="bfff1-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfff1-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bfff1-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bfff1-137">Parameter</span></span>    | <span data-ttu-id="bfff1-138">型</span><span class="sxs-lookup"><span data-stu-id="bfff1-138">Type</span></span>   |<span data-ttu-id="bfff1-139">説明</span><span class="sxs-lookup"><span data-stu-id="bfff1-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfff1-140">comment</span><span class="sxs-lookup"><span data-stu-id="bfff1-140">comment</span></span>|<span data-ttu-id="bfff1-141">String</span><span class="sxs-lookup"><span data-stu-id="bfff1-141">String</span></span>|<span data-ttu-id="bfff1-142">すべての出席者に送信されるキャンセルに関してのコメント。</span><span class="sxs-lookup"><span data-stu-id="bfff1-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="bfff1-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bfff1-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="bfff1-144">応答</span><span class="sxs-lookup"><span data-stu-id="bfff1-144">Response</span></span>

<span data-ttu-id="bfff1-p107">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bfff1-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfff1-147">例</span><span class="sxs-lookup"><span data-stu-id="bfff1-147">Example</span></span>
<span data-ttu-id="bfff1-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bfff1-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bfff1-149">要求</span><span class="sxs-lookup"><span data-stu-id="bfff1-149">Request</span></span>
<span data-ttu-id="bfff1-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bfff1-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bfff1-151">応答</span><span class="sxs-lookup"><span data-stu-id="bfff1-151">Response</span></span>
<span data-ttu-id="bfff1-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bfff1-152">Here is an example of the response.</span></span>
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
