---
title: Delete calendar
description: 既定の予定表以外の予定を削除します。
ms.openlocfilehash: ea020f5e8d10414fffceb0e44fd6e6f39ada294e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020958"
---
# <a name="delete-calendar"></a><span data-ttu-id="469c9-103">Delete calendar</span><span class="sxs-lookup"><span data-stu-id="469c9-103">Delete calendar</span></span>

<span data-ttu-id="469c9-104">既定の予定表以外の予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="469c9-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="469c9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="469c9-105">Permissions</span></span>
<span data-ttu-id="469c9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="469c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="469c9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="469c9-108">Permission type</span></span>      | <span data-ttu-id="469c9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="469c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="469c9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="469c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="469c9-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469c9-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="469c9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="469c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="469c9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469c9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="469c9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="469c9-114">Application</span></span> | <span data-ttu-id="469c9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469c9-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="469c9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="469c9-116">HTTP request</span></span>
<span data-ttu-id="469c9-117"><!-- { "blockType": "ignored" } -->デフォルトの[calendarGroup](../resources/calendargroup.md)での既定の予定表以外のユーザーの[予定表](../resources/calendar.md)です。</span><span class="sxs-lookup"><span data-stu-id="469c9-117"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="469c9-118">指定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外の [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="469c9-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="469c9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="469c9-119">Request headers</span></span>
| <span data-ttu-id="469c9-120">名前</span><span class="sxs-lookup"><span data-stu-id="469c9-120">Name</span></span>           |  <span data-ttu-id="469c9-121">型</span><span class="sxs-lookup"><span data-stu-id="469c9-121">Type</span></span>    | <span data-ttu-id="469c9-122">説明</span><span class="sxs-lookup"><span data-stu-id="469c9-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="469c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="469c9-123">Authorization</span></span>  |  <span data-ttu-id="469c9-124">string</span><span class="sxs-lookup"><span data-stu-id="469c9-124">string</span></span>  | <span data-ttu-id="469c9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="469c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="469c9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="469c9-127">Request body</span></span>
<span data-ttu-id="469c9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="469c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="469c9-129">応答</span><span class="sxs-lookup"><span data-stu-id="469c9-129">Response</span></span>

<span data-ttu-id="469c9-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="469c9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="469c9-132">例</span><span class="sxs-lookup"><span data-stu-id="469c9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="469c9-133">要求</span><span class="sxs-lookup"><span data-stu-id="469c9-133">Request</span></span>
<span data-ttu-id="469c9-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="469c9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="469c9-135">応答</span><span class="sxs-lookup"><span data-stu-id="469c9-135">Response</span></span>
<span data-ttu-id="469c9-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="469c9-136">Here is an example of the response.</span></span> 
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
