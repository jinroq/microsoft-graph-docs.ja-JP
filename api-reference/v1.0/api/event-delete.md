---
title: イベントの削除
description: イベントを削除します。
ms.openlocfilehash: 6f9ee81f60fc3a45018cb137288bad7f22fb98a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023731"
---
# <a name="delete-event"></a><span data-ttu-id="873fb-103">イベントの削除</span><span class="sxs-lookup"><span data-stu-id="873fb-103">Delete event</span></span>

<span data-ttu-id="873fb-104">イベントを削除します。</span><span class="sxs-lookup"><span data-stu-id="873fb-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="873fb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="873fb-105">Permissions</span></span>
<span data-ttu-id="873fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="873fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="873fb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="873fb-108">Permission type</span></span>      | <span data-ttu-id="873fb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="873fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="873fb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="873fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="873fb-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="873fb-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="873fb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="873fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="873fb-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="873fb-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="873fb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="873fb-114">Application</span></span> | <span data-ttu-id="873fb-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="873fb-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="873fb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="873fb-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="873fb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="873fb-117">Request headers</span></span>
| <span data-ttu-id="873fb-118">名前</span><span class="sxs-lookup"><span data-stu-id="873fb-118">Name</span></span>       | <span data-ttu-id="873fb-119">型</span><span class="sxs-lookup"><span data-stu-id="873fb-119">Type</span></span> | <span data-ttu-id="873fb-120">説明</span><span class="sxs-lookup"><span data-stu-id="873fb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="873fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="873fb-121">Authorization</span></span>  | <span data-ttu-id="873fb-122">string</span><span class="sxs-lookup"><span data-stu-id="873fb-122">string</span></span>  | <span data-ttu-id="873fb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="873fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="873fb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="873fb-125">Request body</span></span>
<span data-ttu-id="873fb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="873fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="873fb-127">応答</span><span class="sxs-lookup"><span data-stu-id="873fb-127">Response</span></span>

<span data-ttu-id="873fb-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="873fb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="873fb-130">例</span><span class="sxs-lookup"><span data-stu-id="873fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="873fb-131">要求</span><span class="sxs-lookup"><span data-stu-id="873fb-131">Request</span></span>
<span data-ttu-id="873fb-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="873fb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="873fb-133">応答</span><span class="sxs-lookup"><span data-stu-id="873fb-133">Response</span></span>
<span data-ttu-id="873fb-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="873fb-134">Here is an example of the response.</span></span> 
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