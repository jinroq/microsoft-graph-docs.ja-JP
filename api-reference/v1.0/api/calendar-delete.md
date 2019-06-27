---
title: Delete calendar
description: 既定の予定表以外の予定を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 97c60f04ef708718125bce02ccfae643f710651b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264814"
---
# <a name="delete-calendar"></a><span data-ttu-id="675d8-103">Delete calendar</span><span class="sxs-lookup"><span data-stu-id="675d8-103">Delete calendar</span></span>

<span data-ttu-id="675d8-104">既定の予定表以外の予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="675d8-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="675d8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="675d8-105">Permissions</span></span>
<span data-ttu-id="675d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="675d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="675d8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="675d8-108">Permission type</span></span>      | <span data-ttu-id="675d8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="675d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="675d8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="675d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="675d8-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="675d8-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="675d8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="675d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="675d8-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="675d8-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="675d8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="675d8-114">Application</span></span> | <span data-ttu-id="675d8-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="675d8-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="675d8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="675d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="675d8-117">既定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外のユーザーの [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="675d8-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="675d8-118">指定 [calendarGroup](../resources/calendargroup.md) 内の既定の予定表以外の [予定表](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="675d8-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="675d8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="675d8-119">Request headers</span></span>
| <span data-ttu-id="675d8-120">名前</span><span class="sxs-lookup"><span data-stu-id="675d8-120">Name</span></span>           |  <span data-ttu-id="675d8-121">型</span><span class="sxs-lookup"><span data-stu-id="675d8-121">Type</span></span>    | <span data-ttu-id="675d8-122">説明</span><span class="sxs-lookup"><span data-stu-id="675d8-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="675d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="675d8-123">Authorization</span></span>  |  <span data-ttu-id="675d8-124">string</span><span class="sxs-lookup"><span data-stu-id="675d8-124">string</span></span>  | <span data-ttu-id="675d8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="675d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="675d8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="675d8-127">Request body</span></span>
<span data-ttu-id="675d8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="675d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="675d8-129">応答</span><span class="sxs-lookup"><span data-stu-id="675d8-129">Response</span></span>

<span data-ttu-id="675d8-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="675d8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="675d8-132">例</span><span class="sxs-lookup"><span data-stu-id="675d8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="675d8-133">要求</span><span class="sxs-lookup"><span data-stu-id="675d8-133">Request</span></span>
<span data-ttu-id="675d8-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="675d8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="675d8-135">応答</span><span class="sxs-lookup"><span data-stu-id="675d8-135">Response</span></span>
<span data-ttu-id="675d8-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="675d8-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="675d8-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="675d8-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="675d8-138">C#</span><span class="sxs-lookup"><span data-stu-id="675d8-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="675d8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="675d8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="675d8-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="675d8-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_calendar-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
