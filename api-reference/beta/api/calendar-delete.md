---
title: Delete calendar
description: 既定の予定表以外の予定を削除します。
ms.openlocfilehash: 4d2d2e755a240e35f73a9c8e292d52441c14a25a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066714"
---
# <a name="delete-calendar"></a><span data-ttu-id="7f41e-103">Delete calendar</span><span class="sxs-lookup"><span data-stu-id="7f41e-103">Delete calendar</span></span>

> <span data-ttu-id="7f41e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f41e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f41e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f41e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f41e-106">既定の予定表以外の予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="7f41e-106">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f41e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f41e-107">Permissions</span></span>
<span data-ttu-id="7f41e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f41e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f41e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f41e-110">Permission type</span></span>      | <span data-ttu-id="7f41e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f41e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f41e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f41e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f41e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f41e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7f41e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f41e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f41e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f41e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7f41e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f41e-116">Application</span></span> | <span data-ttu-id="7f41e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f41e-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f41e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f41e-118">HTTP request</span></span>
<span data-ttu-id="7f41e-119"><!-- { "blockType": "ignored" } -->デフォルトの[calendarGroup](../resources/calendargroup.md)での既定の予定表以外のユーザーの[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="7f41e-119"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="7f41e-120">指定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外の [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="7f41e-120">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f41e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f41e-121">Request headers</span></span>
| <span data-ttu-id="7f41e-122">名前</span><span class="sxs-lookup"><span data-stu-id="7f41e-122">Name</span></span>           |  <span data-ttu-id="7f41e-123">型</span><span class="sxs-lookup"><span data-stu-id="7f41e-123">Type</span></span>    | <span data-ttu-id="7f41e-124">説明</span><span class="sxs-lookup"><span data-stu-id="7f41e-124">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="7f41e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f41e-125">Authorization</span></span>  |  <span data-ttu-id="7f41e-126">string</span><span class="sxs-lookup"><span data-stu-id="7f41e-126">string</span></span>  | <span data-ttu-id="7f41e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7f41e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f41e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f41e-129">Request body</span></span>
<span data-ttu-id="7f41e-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f41e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f41e-131">応答</span><span class="sxs-lookup"><span data-stu-id="7f41e-131">Response</span></span>

<span data-ttu-id="7f41e-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7f41e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f41e-134">例</span><span class="sxs-lookup"><span data-stu-id="7f41e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f41e-135">要求</span><span class="sxs-lookup"><span data-stu-id="7f41e-135">Request</span></span>
<span data-ttu-id="7f41e-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f41e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="7f41e-137">応答</span><span class="sxs-lookup"><span data-stu-id="7f41e-137">Response</span></span>
<span data-ttu-id="7f41e-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7f41e-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
