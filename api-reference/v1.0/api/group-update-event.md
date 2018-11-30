---
title: イベントの更新
description: event オブジェクトを更新します。
ms.openlocfilehash: e06f08b0c1f0703904c2418ac490be2100e39619
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022356"
---
# <a name="update-event"></a><span data-ttu-id="d6044-103">イベントを更新する</span><span class="sxs-lookup"><span data-stu-id="d6044-103">Update event</span></span>
<span data-ttu-id="d6044-104">[event](../resources/event.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6044-104">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6044-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6044-105">Permissions</span></span>
<span data-ttu-id="d6044-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6044-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6044-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6044-108">Permission type</span></span>      | <span data-ttu-id="d6044-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6044-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6044-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6044-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6044-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6044-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6044-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6044-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6044-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6044-113">Not supported.</span></span>    |
|<span data-ttu-id="d6044-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6044-114">Application</span></span> | <span data-ttu-id="d6044-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6044-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6044-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6044-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6044-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6044-117">Request headers</span></span>
| <span data-ttu-id="d6044-118">名前</span><span class="sxs-lookup"><span data-stu-id="d6044-118">Name</span></span>       | <span data-ttu-id="d6044-119">型</span><span class="sxs-lookup"><span data-stu-id="d6044-119">Type</span></span> | <span data-ttu-id="d6044-120">説明</span><span class="sxs-lookup"><span data-stu-id="d6044-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6044-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6044-121">Authorization</span></span>  | <span data-ttu-id="d6044-122">string</span><span class="sxs-lookup"><span data-stu-id="d6044-122">string</span></span>  | <span data-ttu-id="d6044-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6044-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6044-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6044-125">Request body</span></span>
<span data-ttu-id="d6044-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d6044-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d6044-129">応答</span><span class="sxs-lookup"><span data-stu-id="d6044-129">Response</span></span>
<span data-ttu-id="d6044-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d6044-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6044-131">例</span><span class="sxs-lookup"><span data-stu-id="d6044-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d6044-132">要求</span><span class="sxs-lookup"><span data-stu-id="d6044-132">Request</span></span>
<span data-ttu-id="d6044-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6044-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="d6044-134">応答</span><span class="sxs-lookup"><span data-stu-id="d6044-134">Response</span></span>
<span data-ttu-id="d6044-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6044-135">The following is an example of the response.</span></span>

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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->