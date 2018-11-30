---
title: HistoryItem を削除します。
description: 既存のユーザー アクティビティの既存の履歴項目を削除します。
ms.openlocfilehash: bf8d8c064a3a29aec8f59a2d4de5ae6732d0f0e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068992"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="66d36-103">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="66d36-103">Delete a historyItem</span></span>

> <span data-ttu-id="66d36-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="66d36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66d36-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66d36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66d36-106">既存のユーザー アクティビティの既存の履歴項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="66d36-106">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="66d36-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66d36-107">Permissions</span></span>

<span data-ttu-id="66d36-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66d36-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66d36-110">Permission type</span></span>      | <span data-ttu-id="66d36-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66d36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d36-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66d36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66d36-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="66d36-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="66d36-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66d36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d36-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="66d36-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="66d36-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66d36-116">Application</span></span> | <span data-ttu-id="66d36-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66d36-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d36-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66d36-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="66d36-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66d36-119">Request headers</span></span>

|<span data-ttu-id="66d36-120">名前</span><span class="sxs-lookup"><span data-stu-id="66d36-120">Name</span></span> | <span data-ttu-id="66d36-121">型</span><span class="sxs-lookup"><span data-stu-id="66d36-121">Type</span></span> | <span data-ttu-id="66d36-122">説明</span><span class="sxs-lookup"><span data-stu-id="66d36-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="66d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d36-123">Authorization</span></span> | <span data-ttu-id="66d36-124">string</span><span class="sxs-lookup"><span data-stu-id="66d36-124">string</span></span> | <span data-ttu-id="66d36-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66d36-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d36-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="66d36-127">Request body</span></span>

<span data-ttu-id="66d36-128">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="66d36-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="66d36-129">応答</span><span class="sxs-lookup"><span data-stu-id="66d36-129">Response</span></span>

<span data-ttu-id="66d36-130">かどうかは成功すると、このメソッドが返されます、 `204 No Content` 、履歴項目が削除された場合の応答コード。</span><span class="sxs-lookup"><span data-stu-id="66d36-130">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="66d36-131">例</span><span class="sxs-lookup"><span data-stu-id="66d36-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66d36-132">要求</span><span class="sxs-lookup"><span data-stu-id="66d36-132">Request</span></span>

<span data-ttu-id="66d36-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66d36-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="66d36-134">応答</span><span class="sxs-lookup"><span data-stu-id="66d36-134">Response</span></span>

<span data-ttu-id="66d36-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="66d36-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->