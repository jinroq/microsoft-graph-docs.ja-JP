---
title: イベントの削除
description: イベントを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ae39e73a9aa81d1b86701017ef2805f33f7d4c17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550078"
---
# <a name="delete-event"></a><span data-ttu-id="ae6fc-103">イベントを削除する</span><span class="sxs-lookup"><span data-stu-id="ae6fc-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae6fc-104">イベントを削除します。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae6fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae6fc-105">Permissions</span></span>
<span data-ttu-id="ae6fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae6fc-108">Permission type</span></span>      | <span data-ttu-id="ae6fc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae6fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae6fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae6fc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6fc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ae6fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae6fc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6fc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ae6fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae6fc-114">Application</span></span> | <span data-ttu-id="ae6fc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6fc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae6fc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae6fc-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ae6fc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6fc-117">Request headers</span></span>
| <span data-ttu-id="ae6fc-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae6fc-118">Name</span></span>       | <span data-ttu-id="ae6fc-119">型</span><span class="sxs-lookup"><span data-stu-id="ae6fc-119">Type</span></span> | <span data-ttu-id="ae6fc-120">説明</span><span class="sxs-lookup"><span data-stu-id="ae6fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae6fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6fc-121">Authorization</span></span>  | <span data-ttu-id="ae6fc-122">string</span><span class="sxs-lookup"><span data-stu-id="ae6fc-122">string</span></span>  | <span data-ttu-id="ae6fc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae6fc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae6fc-125">Request body</span></span>
<span data-ttu-id="ae6fc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae6fc-127">応答</span><span class="sxs-lookup"><span data-stu-id="ae6fc-127">Response</span></span>

<span data-ttu-id="ae6fc-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6fc-130">例</span><span class="sxs-lookup"><span data-stu-id="ae6fc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae6fc-131">要求</span><span class="sxs-lookup"><span data-stu-id="ae6fc-131">Request</span></span>
<span data-ttu-id="ae6fc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="ae6fc-133">応答</span><span class="sxs-lookup"><span data-stu-id="ae6fc-133">Response</span></span>
<span data-ttu-id="ae6fc-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ae6fc-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
