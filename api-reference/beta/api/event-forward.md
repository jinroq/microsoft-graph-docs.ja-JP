---
title: 'イベント: 転送'
description: 'このアクションにより、会議イベントの開催者または出席者が '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f1b3e1f089d927aeb21ca80ff77edda63121c60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464343"
---
# <a name="event-forward"></a><span data-ttu-id="cc86c-103">イベント: 転送</span><span class="sxs-lookup"><span data-stu-id="cc86c-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc86c-104">このアクションにより、会議[イベント](../resources/event.md)の開催者または出席者は、新しい受信者に会議出席依頼を転送することができます。</span><span class="sxs-lookup"><span data-stu-id="cc86c-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="cc86c-105">会議イベントが出席者の Office 365 メールボックスから別の受信者に転送された場合、この操作を行うと、転送先を開催者に通知するメッセージも送信され、受信者は会議イベントの開催者のコピーに追加されます。</span><span class="sxs-lookup"><span data-stu-id="cc86c-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="cc86c-106">この利便性は、Outlook.com アカウントから転送する場合には使用できません。</span><span class="sxs-lookup"><span data-stu-id="cc86c-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="cc86c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc86c-107">Permissions</span></span>
<span data-ttu-id="cc86c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc86c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc86c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc86c-110">Permission type</span></span>      | <span data-ttu-id="cc86c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc86c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc86c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc86c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc86c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cc86c-113">Calendars.Read</span></span>    |
|<span data-ttu-id="cc86c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc86c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc86c-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cc86c-115">Calendars.Read</span></span>    |
|<span data-ttu-id="cc86c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc86c-116">Application</span></span> | <span data-ttu-id="cc86c-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cc86c-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc86c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc86c-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="cc86c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc86c-119">Request headers</span></span>
| <span data-ttu-id="cc86c-120">名前</span><span class="sxs-lookup"><span data-stu-id="cc86c-120">Name</span></span>       | <span data-ttu-id="cc86c-121">型</span><span class="sxs-lookup"><span data-stu-id="cc86c-121">Type</span></span> | <span data-ttu-id="cc86c-122">説明</span><span class="sxs-lookup"><span data-stu-id="cc86c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc86c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc86c-123">Authorization</span></span>  | <span data-ttu-id="cc86c-124">string</span><span class="sxs-lookup"><span data-stu-id="cc86c-124">string</span></span>  | <span data-ttu-id="cc86c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc86c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc86c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc86c-127">Content-Type</span></span> | <span data-ttu-id="cc86c-128">string</span><span class="sxs-lookup"><span data-stu-id="cc86c-128">string</span></span>  | <span data-ttu-id="cc86c-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="cc86c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc86c-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc86c-131">Request body</span></span>
<span data-ttu-id="cc86c-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc86c-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc86c-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc86c-133">Parameter</span></span>    | <span data-ttu-id="cc86c-134">型</span><span class="sxs-lookup"><span data-stu-id="cc86c-134">Type</span></span>   |<span data-ttu-id="cc86c-135">説明</span><span class="sxs-lookup"><span data-stu-id="cc86c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc86c-136">Comment</span><span class="sxs-lookup"><span data-stu-id="cc86c-136">Comment</span></span>|<span data-ttu-id="cc86c-137">String</span><span class="sxs-lookup"><span data-stu-id="cc86c-137">String</span></span>|<span data-ttu-id="cc86c-p105">含めるコメントです。空の文字列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cc86c-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="cc86c-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="cc86c-140">ToRecipients</span></span>|<span data-ttu-id="cc86c-141">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="cc86c-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="cc86c-142">イベントを転送する受信者の一覧。</span><span class="sxs-lookup"><span data-stu-id="cc86c-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="cc86c-143">応答</span><span class="sxs-lookup"><span data-stu-id="cc86c-143">Response</span></span>

<span data-ttu-id="cc86c-p106">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="cc86c-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc86c-146">例</span><span class="sxs-lookup"><span data-stu-id="cc86c-146">Example</span></span>
<span data-ttu-id="cc86c-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cc86c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc86c-148">要求</span><span class="sxs-lookup"><span data-stu-id="cc86c-148">Request</span></span>
<span data-ttu-id="cc86c-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc86c-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="cc86c-150">応答</span><span class="sxs-lookup"><span data-stu-id="cc86c-150">Response</span></span>
<span data-ttu-id="cc86c-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="cc86c-151">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/event-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
