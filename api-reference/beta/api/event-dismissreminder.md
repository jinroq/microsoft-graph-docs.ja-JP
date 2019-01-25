---
title: 'イベント: dismissReminder'
description: ユーザーの予定表でイベントをトリガーされたアラームを閉じます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 885a285e3c35f59b0fde76be5c84ae152a2ad13a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523051"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="0ab70-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="0ab70-103">event: dismissReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ab70-104">ユーザー[の予定表](../resources/calendar.md)の[イベント](../resources/event.md)のトリガーされたアラームを閉じます。</span><span class="sxs-lookup"><span data-stu-id="0ab70-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ab70-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0ab70-105">Permissions</span></span>
<span data-ttu-id="0ab70-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ab70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab70-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ab70-108">Permission type</span></span>      | <span data-ttu-id="0ab70-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ab70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ab70-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ab70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ab70-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab70-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ab70-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ab70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ab70-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab70-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ab70-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ab70-114">Application</span></span> | <span data-ttu-id="0ab70-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ab70-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ab70-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ab70-116">HTTP request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0ab70-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ab70-117">Request headers</span></span>

| <span data-ttu-id="0ab70-118">名前</span><span class="sxs-lookup"><span data-stu-id="0ab70-118">Name</span></span>       | <span data-ttu-id="0ab70-119">型</span><span class="sxs-lookup"><span data-stu-id="0ab70-119">Type</span></span> | <span data-ttu-id="0ab70-120">説明</span><span class="sxs-lookup"><span data-stu-id="0ab70-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ab70-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab70-121">Authorization</span></span>  | <span data-ttu-id="0ab70-122">string</span><span class="sxs-lookup"><span data-stu-id="0ab70-122">string</span></span>  | <span data-ttu-id="0ab70-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0ab70-p102">Bearer {token}. Required.</span></span> |


## <a name="response"></a><span data-ttu-id="0ab70-125">応答</span><span class="sxs-lookup"><span data-stu-id="0ab70-125">Response</span></span>

<span data-ttu-id="0ab70-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0ab70-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ab70-128">例</span><span class="sxs-lookup"><span data-stu-id="0ab70-128">Example</span></span>

<span data-ttu-id="0ab70-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0ab70-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0ab70-130">要求</span><span class="sxs-lookup"><span data-stu-id="0ab70-130">Request</span></span>
<span data-ttu-id="0ab70-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ab70-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/dismissReminder
```

### <a name="response"></a><span data-ttu-id="0ab70-132">応答</span><span class="sxs-lookup"><span data-stu-id="0ab70-132">Response</span></span>
<span data-ttu-id="0ab70-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0ab70-133">Here is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/event-dismissreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
