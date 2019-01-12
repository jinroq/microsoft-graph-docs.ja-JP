---
title: 'イベント: dismissReminder'
description: ユーザーの予定表でイベントをトリガーされたアラームを閉じます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cf2421db56babd394a3c011fb9bd4db9f83cb823
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990321"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="8897b-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="8897b-103">event: dismissReminder</span></span>

<span data-ttu-id="8897b-104">ユーザー[の予定表](../resources/calendar.md)の[イベント](../resources/event.md)のトリガーされたアラームを閉じます。</span><span class="sxs-lookup"><span data-stu-id="8897b-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8897b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8897b-105">Permissions</span></span>
<span data-ttu-id="8897b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8897b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8897b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8897b-108">Permission type</span></span>      | <span data-ttu-id="8897b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8897b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8897b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8897b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8897b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8897b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8897b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8897b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8897b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8897b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8897b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8897b-114">Application</span></span> | <span data-ttu-id="8897b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8897b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8897b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8897b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="8897b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8897b-117">Request headers</span></span>
| <span data-ttu-id="8897b-118">名前</span><span class="sxs-lookup"><span data-stu-id="8897b-118">Name</span></span>       | <span data-ttu-id="8897b-119">種類</span><span class="sxs-lookup"><span data-stu-id="8897b-119">Type</span></span> | <span data-ttu-id="8897b-120">説明</span><span class="sxs-lookup"><span data-stu-id="8897b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8897b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8897b-121">Authorization</span></span>  | <span data-ttu-id="8897b-122">string</span><span class="sxs-lookup"><span data-stu-id="8897b-122">string</span></span>  | <span data-ttu-id="8897b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8897b-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="8897b-125">応答</span><span class="sxs-lookup"><span data-stu-id="8897b-125">Response</span></span>

<span data-ttu-id="8897b-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8897b-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8897b-128">例</span><span class="sxs-lookup"><span data-stu-id="8897b-128">Example</span></span>

<span data-ttu-id="8897b-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8897b-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8897b-130">要求</span><span class="sxs-lookup"><span data-stu-id="8897b-130">Request</span></span>
<span data-ttu-id="8897b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8897b-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="8897b-132">応答</span><span class="sxs-lookup"><span data-stu-id="8897b-132">Response</span></span>
<span data-ttu-id="8897b-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8897b-133">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
