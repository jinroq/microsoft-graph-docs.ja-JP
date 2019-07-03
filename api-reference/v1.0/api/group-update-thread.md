---
title: 会話スレッドを更新する
description: thread オブジェクトを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f95969a16437bdbb9a8b300c1a8cdd0d9ffe52d9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450661"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="90aba-103">会話スレッドを更新する</span><span class="sxs-lookup"><span data-stu-id="90aba-103">Update conversation thread</span></span>
<span data-ttu-id="90aba-104">[thread](../resources/conversationthread.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="90aba-104">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90aba-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="90aba-105">Permissions</span></span>
<span data-ttu-id="90aba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90aba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90aba-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90aba-108">Permission type</span></span>      | <span data-ttu-id="90aba-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="90aba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90aba-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90aba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90aba-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90aba-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90aba-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90aba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90aba-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aba-113">Not supported.</span></span>    |
|<span data-ttu-id="90aba-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90aba-114">Application</span></span> | <span data-ttu-id="90aba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90aba-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90aba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90aba-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90aba-117">Request headers</span></span>
| <span data-ttu-id="90aba-118">名前</span><span class="sxs-lookup"><span data-stu-id="90aba-118">Name</span></span>       | <span data-ttu-id="90aba-119">型</span><span class="sxs-lookup"><span data-stu-id="90aba-119">Type</span></span> | <span data-ttu-id="90aba-120">説明</span><span class="sxs-lookup"><span data-stu-id="90aba-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="90aba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90aba-121">Authorization</span></span>  | <span data-ttu-id="90aba-122">string</span><span class="sxs-lookup"><span data-stu-id="90aba-122">string</span></span>  | <span data-ttu-id="90aba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="90aba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90aba-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="90aba-125">Request body</span></span>
<span data-ttu-id="90aba-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="90aba-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="90aba-129">応答</span><span class="sxs-lookup"><span data-stu-id="90aba-129">Response</span></span>
<span data-ttu-id="90aba-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="90aba-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90aba-131">例</span><span class="sxs-lookup"><span data-stu-id="90aba-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="90aba-132">要求</span><span class="sxs-lookup"><span data-stu-id="90aba-132">Request</span></span>
<span data-ttu-id="90aba-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="90aba-133">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="90aba-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="90aba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90aba-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="90aba-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90aba-136">応答</span><span class="sxs-lookup"><span data-stu-id="90aba-136">Response</span></span>
<span data-ttu-id="90aba-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="90aba-137">The following is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
