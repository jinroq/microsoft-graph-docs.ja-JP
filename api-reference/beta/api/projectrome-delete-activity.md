---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 8b4bf0b09cb5796e1db8e22ced7e471bdd5117f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925750"
---
# <a name="delete-an-activity"></a><span data-ttu-id="f5fcf-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="f5fcf-103">Delete an activity</span></span>

> <span data-ttu-id="f5fcf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5fcf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5fcf-106">アプリの既存のユーザーのアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5fcf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5fcf-107">Permissions</span></span>

<span data-ttu-id="f5fcf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f5fcf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5fcf-110">Permission type</span></span>      | <span data-ttu-id="f5fcf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5fcf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5fcf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5fcf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5fcf-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f5fcf-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f5fcf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5fcf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fcf-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f5fcf-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f5fcf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5fcf-116">Application</span></span> | <span data-ttu-id="f5fcf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5fcf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5fcf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5fcf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5fcf-119">Request headers</span></span>

|<span data-ttu-id="f5fcf-120">名前</span><span class="sxs-lookup"><span data-stu-id="f5fcf-120">Name</span></span> | <span data-ttu-id="f5fcf-121">種類</span><span class="sxs-lookup"><span data-stu-id="f5fcf-121">Type</span></span> | <span data-ttu-id="f5fcf-122">説明</span><span class="sxs-lookup"><span data-stu-id="f5fcf-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f5fcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5fcf-123">Authorization</span></span> | <span data-ttu-id="f5fcf-124">string</span><span class="sxs-lookup"><span data-stu-id="f5fcf-124">string</span></span> | <span data-ttu-id="f5fcf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5fcf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5fcf-127">Request body</span></span>

<span data-ttu-id="f5fcf-128">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="f5fcf-129">応答</span><span class="sxs-lookup"><span data-stu-id="f5fcf-129">Response</span></span>

<span data-ttu-id="f5fcf-130">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="f5fcf-131">例</span><span class="sxs-lookup"><span data-stu-id="f5fcf-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f5fcf-132">要求</span><span class="sxs-lookup"><span data-stu-id="f5fcf-132">Request</span></span>

<span data-ttu-id="f5fcf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="f5fcf-134">応答</span><span class="sxs-lookup"><span data-stu-id="f5fcf-134">Response</span></span>

<span data-ttu-id="f5fcf-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f5fcf-135">Here is an example of the response.</span></span>

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
