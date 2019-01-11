---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
localization_priority: Normal
ms.openlocfilehash: 92b927dbb568221003fdaff108640cf24520d182
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819552"
---
# <a name="delete-an-activity"></a><span data-ttu-id="a901d-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="a901d-103">Delete an activity</span></span>

> <span data-ttu-id="a901d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a901d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a901d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a901d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a901d-106">アプリの既存のユーザーのアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="a901d-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a901d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a901d-107">Permissions</span></span>

<span data-ttu-id="a901d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a901d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a901d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a901d-110">Permission type</span></span>      | <span data-ttu-id="a901d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a901d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a901d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a901d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a901d-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a901d-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a901d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a901d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a901d-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a901d-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a901d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a901d-116">Application</span></span> | <span data-ttu-id="a901d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a901d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a901d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a901d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a901d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a901d-119">Request headers</span></span>

|<span data-ttu-id="a901d-120">名前</span><span class="sxs-lookup"><span data-stu-id="a901d-120">Name</span></span> | <span data-ttu-id="a901d-121">種類</span><span class="sxs-lookup"><span data-stu-id="a901d-121">Type</span></span> | <span data-ttu-id="a901d-122">説明</span><span class="sxs-lookup"><span data-stu-id="a901d-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a901d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a901d-123">Authorization</span></span> | <span data-ttu-id="a901d-124">string</span><span class="sxs-lookup"><span data-stu-id="a901d-124">string</span></span> | <span data-ttu-id="a901d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a901d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a901d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a901d-127">Request body</span></span>

<span data-ttu-id="a901d-128">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="a901d-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="a901d-129">応答</span><span class="sxs-lookup"><span data-stu-id="a901d-129">Response</span></span>

<span data-ttu-id="a901d-130">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="a901d-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="a901d-131">例</span><span class="sxs-lookup"><span data-stu-id="a901d-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a901d-132">要求</span><span class="sxs-lookup"><span data-stu-id="a901d-132">Request</span></span>

<span data-ttu-id="a901d-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a901d-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="a901d-134">応答</span><span class="sxs-lookup"><span data-stu-id="a901d-134">Response</span></span>

<span data-ttu-id="a901d-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a901d-135">Here is an example of the response.</span></span>

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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
