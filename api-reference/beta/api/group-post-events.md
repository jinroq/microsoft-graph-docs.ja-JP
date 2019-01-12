---
title: イベントを作成する
description: この API を使用して、新しいイベントを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 83d41f083a19ce813205dccc0056b2de16935541
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915180"
---
# <a name="create-event"></a><span data-ttu-id="f66e7-103">イベントを作成する</span><span class="sxs-lookup"><span data-stu-id="f66e7-103">Create event</span></span>

> <span data-ttu-id="f66e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f66e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f66e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f66e7-106">この API を使用して、新しい[イベント](../resources/event.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-106">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f66e7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f66e7-107">Permissions</span></span>
<span data-ttu-id="f66e7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f66e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f66e7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f66e7-110">Permission type</span></span>      | <span data-ttu-id="f66e7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f66e7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f66e7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f66e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f66e7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f66e7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f66e7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f66e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f66e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66e7-115">Not supported.</span></span>    |
|<span data-ttu-id="f66e7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f66e7-116">Application</span></span> | <span data-ttu-id="f66e7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66e7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f66e7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f66e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="f66e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f66e7-119">Request headers</span></span>
| <span data-ttu-id="f66e7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f66e7-120">Header</span></span>       | <span data-ttu-id="f66e7-121">値</span><span class="sxs-lookup"><span data-stu-id="f66e7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f66e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66e7-122">Authorization</span></span>  | <span data-ttu-id="f66e7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f66e7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f66e7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f66e7-125">Request body</span></span>
<span data-ttu-id="f66e7-126">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-126">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f66e7-127">応答</span><span class="sxs-lookup"><span data-stu-id="f66e7-127">Response</span></span>
<span data-ttu-id="f66e7-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[イベント](../resources/event.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-128">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f66e7-129">例</span><span class="sxs-lookup"><span data-stu-id="f66e7-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f66e7-130">要求</span><span class="sxs-lookup"><span data-stu-id="f66e7-130">Request</span></span>
<span data-ttu-id="f66e7-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="f66e7-132">要求本文で、[イベント](../resources/event.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-132">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="f66e7-133">応答</span><span class="sxs-lookup"><span data-stu-id="f66e7-133">Response</span></span>
<span data-ttu-id="f66e7-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f66e7-134">The following is an example of the response.</span></span>
><span data-ttu-id="f66e7-135">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f66e7-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f66e7-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f66e7-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
