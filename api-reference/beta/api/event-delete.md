---
title: イベントの削除
description: イベントを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 830568c5abbd02f0083cf45d5172266c2bf20e41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956564"
---
# <a name="delete-event"></a><span data-ttu-id="215d9-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="215d9-103">Delete event</span></span>

> <span data-ttu-id="215d9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="215d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="215d9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="215d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="215d9-106">イベントを削除します。</span><span class="sxs-lookup"><span data-stu-id="215d9-106">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="215d9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="215d9-107">Permissions</span></span>
<span data-ttu-id="215d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="215d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="215d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="215d9-110">Permission type</span></span>      | <span data-ttu-id="215d9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="215d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="215d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="215d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="215d9-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="215d9-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="215d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="215d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="215d9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="215d9-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="215d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="215d9-116">Application</span></span> | <span data-ttu-id="215d9-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="215d9-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="215d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="215d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="215d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="215d9-119">Request headers</span></span>
| <span data-ttu-id="215d9-120">名前</span><span class="sxs-lookup"><span data-stu-id="215d9-120">Name</span></span>       | <span data-ttu-id="215d9-121">種類</span><span class="sxs-lookup"><span data-stu-id="215d9-121">Type</span></span> | <span data-ttu-id="215d9-122">説明</span><span class="sxs-lookup"><span data-stu-id="215d9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="215d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="215d9-123">Authorization</span></span>  | <span data-ttu-id="215d9-124">string</span><span class="sxs-lookup"><span data-stu-id="215d9-124">string</span></span>  | <span data-ttu-id="215d9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="215d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="215d9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="215d9-127">Request body</span></span>
<span data-ttu-id="215d9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="215d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="215d9-129">応答</span><span class="sxs-lookup"><span data-stu-id="215d9-129">Response</span></span>

<span data-ttu-id="215d9-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="215d9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="215d9-132">例</span><span class="sxs-lookup"><span data-stu-id="215d9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="215d9-133">要求</span><span class="sxs-lookup"><span data-stu-id="215d9-133">Request</span></span>
<span data-ttu-id="215d9-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="215d9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="215d9-135">応答</span><span class="sxs-lookup"><span data-stu-id="215d9-135">Response</span></span>
<span data-ttu-id="215d9-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="215d9-136">Here is an example of the response.</span></span> 
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
