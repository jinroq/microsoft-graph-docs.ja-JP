---
title: 'イベント: dismissReminder'
description: ユーザーの予定表のイベントに対してトリガーされたアラームを消します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dd10d8a94e2661f2006ccb10c4a823c4afc3fdb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324410"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="827dc-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="827dc-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="827dc-104">ユーザーの[予定表](../resources/calendar.md)の[イベント](../resources/event.md)に対してトリガーされたアラームを消します。</span><span class="sxs-lookup"><span data-stu-id="827dc-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="827dc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="827dc-105">Permissions</span></span>
<span data-ttu-id="827dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="827dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="827dc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="827dc-108">Permission type</span></span>      | <span data-ttu-id="827dc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="827dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="827dc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="827dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="827dc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="827dc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="827dc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="827dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="827dc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="827dc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="827dc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="827dc-114">Application</span></span> | <span data-ttu-id="827dc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="827dc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="827dc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="827dc-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="827dc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="827dc-117">Request headers</span></span>

| <span data-ttu-id="827dc-118">名前</span><span class="sxs-lookup"><span data-stu-id="827dc-118">Name</span></span>       | <span data-ttu-id="827dc-119">型</span><span class="sxs-lookup"><span data-stu-id="827dc-119">Type</span></span> | <span data-ttu-id="827dc-120">説明</span><span class="sxs-lookup"><span data-stu-id="827dc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="827dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="827dc-121">Authorization</span></span>  | <span data-ttu-id="827dc-122">string</span><span class="sxs-lookup"><span data-stu-id="827dc-122">string</span></span>  | <span data-ttu-id="827dc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="827dc-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="827dc-125">応答</span><span class="sxs-lookup"><span data-stu-id="827dc-125">Response</span></span>

<span data-ttu-id="827dc-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="827dc-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="827dc-128">例</span><span class="sxs-lookup"><span data-stu-id="827dc-128">Example</span></span>

<span data-ttu-id="827dc-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="827dc-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="827dc-130">要求</span><span class="sxs-lookup"><span data-stu-id="827dc-130">Request</span></span>
<span data-ttu-id="827dc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="827dc-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="827dc-132">応答</span><span class="sxs-lookup"><span data-stu-id="827dc-132">Response</span></span>
<span data-ttu-id="827dc-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="827dc-133">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
