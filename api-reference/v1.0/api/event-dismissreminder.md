---
title: 'イベント: dismissReminder'
description: ユーザーの予定表のイベントに対してトリガーされたアラームを消します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b04879b8af87fc58923d6eb8472d8b54ba97d5de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887441"
---
# <a name="event-dismissreminder"></a><span data-ttu-id="dd67b-103">イベント: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="dd67b-103">event: dismissReminder</span></span>

<span data-ttu-id="dd67b-104">ユーザーの[予定表](../resources/calendar.md)の[イベント](../resources/event.md)に対してトリガーされたアラームを消します。</span><span class="sxs-lookup"><span data-stu-id="dd67b-104">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd67b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dd67b-105">Permissions</span></span>
<span data-ttu-id="dd67b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dd67b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd67b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dd67b-108">Permission type</span></span>      | <span data-ttu-id="dd67b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dd67b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd67b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dd67b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd67b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd67b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dd67b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dd67b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd67b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd67b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="dd67b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dd67b-114">Application</span></span> | <span data-ttu-id="dd67b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd67b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd67b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dd67b-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="dd67b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dd67b-117">Request headers</span></span>
| <span data-ttu-id="dd67b-118">名前</span><span class="sxs-lookup"><span data-stu-id="dd67b-118">Name</span></span>       | <span data-ttu-id="dd67b-119">型</span><span class="sxs-lookup"><span data-stu-id="dd67b-119">Type</span></span> | <span data-ttu-id="dd67b-120">説明</span><span class="sxs-lookup"><span data-stu-id="dd67b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dd67b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd67b-121">Authorization</span></span>  | <span data-ttu-id="dd67b-122">string</span><span class="sxs-lookup"><span data-stu-id="dd67b-122">string</span></span>  | <span data-ttu-id="dd67b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dd67b-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="dd67b-125">応答</span><span class="sxs-lookup"><span data-stu-id="dd67b-125">Response</span></span>

<span data-ttu-id="dd67b-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="dd67b-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd67b-128">例</span><span class="sxs-lookup"><span data-stu-id="dd67b-128">Example</span></span>

<span data-ttu-id="dd67b-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dd67b-129">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dd67b-130">要求</span><span class="sxs-lookup"><span data-stu-id="dd67b-130">Request</span></span>
<span data-ttu-id="dd67b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dd67b-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd67b-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="dd67b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd67b-133">C#</span><span class="sxs-lookup"><span data-stu-id="dd67b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-dismissreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd67b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd67b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-dismissreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd67b-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="dd67b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-dismissreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd67b-136">Java</span><span class="sxs-lookup"><span data-stu-id="dd67b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-dismissreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

### <a name="response"></a><span data-ttu-id="dd67b-137">応答</span><span class="sxs-lookup"><span data-stu-id="dd67b-137">Response</span></span>
<span data-ttu-id="dd67b-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dd67b-138">Here is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
