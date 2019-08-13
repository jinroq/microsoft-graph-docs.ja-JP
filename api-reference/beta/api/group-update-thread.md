---
title: 会話スレッドを更新する
description: thread オブジェクトを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 314ed992ca9dafbce7ace3cec27990467609fb76
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323104"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="4d95b-103">会話スレッドを更新する</span><span class="sxs-lookup"><span data-stu-id="4d95b-103">Update conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d95b-104">[thread](../resources/conversationthread.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d95b-104">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d95b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d95b-105">Permissions</span></span>
<span data-ttu-id="4d95b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d95b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d95b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d95b-108">Permission type</span></span>      | <span data-ttu-id="4d95b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d95b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d95b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d95b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d95b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d95b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d95b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d95b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d95b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d95b-113">Not supported.</span></span>    |
|<span data-ttu-id="4d95b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d95b-114">Application</span></span> | <span data-ttu-id="4d95b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d95b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d95b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d95b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4d95b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d95b-117">Request headers</span></span>
| <span data-ttu-id="4d95b-118">名前</span><span class="sxs-lookup"><span data-stu-id="4d95b-118">Name</span></span>       | <span data-ttu-id="4d95b-119">型</span><span class="sxs-lookup"><span data-stu-id="4d95b-119">Type</span></span> | <span data-ttu-id="4d95b-120">説明</span><span class="sxs-lookup"><span data-stu-id="4d95b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4d95b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d95b-121">Authorization</span></span>  | <span data-ttu-id="4d95b-122">string</span><span class="sxs-lookup"><span data-stu-id="4d95b-122">string</span></span>  | <span data-ttu-id="4d95b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d95b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d95b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d95b-125">Request body</span></span>
<span data-ttu-id="4d95b-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4d95b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4d95b-129">応答</span><span class="sxs-lookup"><span data-stu-id="4d95b-129">Response</span></span>
<span data-ttu-id="4d95b-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4d95b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d95b-131">例</span><span class="sxs-lookup"><span data-stu-id="4d95b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4d95b-132">要求</span><span class="sxs-lookup"><span data-stu-id="4d95b-132">Request</span></span>
<span data-ttu-id="4d95b-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d95b-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4d95b-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d95b-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d95b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d95b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4d95b-136">応答</span><span class="sxs-lookup"><span data-stu-id="4d95b-136">Response</span></span>
<span data-ttu-id="4d95b-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4d95b-137">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
