---
title: 会話スレッドを更新する
description: thread オブジェクトを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: defb7560a1d407a60ac813154ebd978f554e9763
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966259"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="150c0-103">会話スレッドを更新する</span><span class="sxs-lookup"><span data-stu-id="150c0-103">Update conversation thread</span></span>

> <span data-ttu-id="150c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="150c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="150c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="150c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="150c0-106">[thread](../resources/conversationthread.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="150c0-106">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="150c0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="150c0-107">Permissions</span></span>
<span data-ttu-id="150c0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="150c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="150c0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="150c0-110">Permission type</span></span>      | <span data-ttu-id="150c0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="150c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="150c0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="150c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="150c0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="150c0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="150c0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="150c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="150c0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="150c0-115">Not supported.</span></span>    |
|<span data-ttu-id="150c0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="150c0-116">Application</span></span> | <span data-ttu-id="150c0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="150c0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="150c0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="150c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="150c0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="150c0-119">Request headers</span></span>
| <span data-ttu-id="150c0-120">名前</span><span class="sxs-lookup"><span data-stu-id="150c0-120">Name</span></span>       | <span data-ttu-id="150c0-121">種類</span><span class="sxs-lookup"><span data-stu-id="150c0-121">Type</span></span> | <span data-ttu-id="150c0-122">説明</span><span class="sxs-lookup"><span data-stu-id="150c0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="150c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="150c0-123">Authorization</span></span>  | <span data-ttu-id="150c0-124">string</span><span class="sxs-lookup"><span data-stu-id="150c0-124">string</span></span>  | <span data-ttu-id="150c0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="150c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="150c0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="150c0-127">Request body</span></span>
<span data-ttu-id="150c0-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="150c0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="150c0-131">応答</span><span class="sxs-lookup"><span data-stu-id="150c0-131">Response</span></span>
<span data-ttu-id="150c0-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="150c0-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="150c0-133">例</span><span class="sxs-lookup"><span data-stu-id="150c0-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="150c0-134">要求</span><span class="sxs-lookup"><span data-stu-id="150c0-134">Request</span></span>
<span data-ttu-id="150c0-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="150c0-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="150c0-136">応答</span><span class="sxs-lookup"><span data-stu-id="150c0-136">Response</span></span>
<span data-ttu-id="150c0-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="150c0-137">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
