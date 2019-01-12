---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: cbe12a373f06c2893a5ca202247865f4ce4a8f52
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966854"
---
# <a name="delete-an-activity"></a><span data-ttu-id="2b083-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="2b083-103">Delete an activity</span></span>

<span data-ttu-id="2b083-104">アプリの既存のユーザーのアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b083-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b083-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b083-105">Permissions</span></span>

<span data-ttu-id="2b083-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b083-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b083-108">Permission type</span></span>      | <span data-ttu-id="2b083-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b083-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b083-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b083-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b083-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="2b083-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="2b083-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b083-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b083-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="2b083-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="2b083-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b083-114">Application</span></span> | <span data-ttu-id="2b083-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b083-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b083-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b083-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b083-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b083-117">Request headers</span></span>

|<span data-ttu-id="2b083-118">名前</span><span class="sxs-lookup"><span data-stu-id="2b083-118">Name</span></span> | <span data-ttu-id="2b083-119">種類</span><span class="sxs-lookup"><span data-stu-id="2b083-119">Type</span></span> | <span data-ttu-id="2b083-120">説明</span><span class="sxs-lookup"><span data-stu-id="2b083-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="2b083-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b083-121">Authorization</span></span> | <span data-ttu-id="2b083-122">string</span><span class="sxs-lookup"><span data-stu-id="2b083-122">string</span></span> | <span data-ttu-id="2b083-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2b083-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b083-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b083-125">Request body</span></span>

<span data-ttu-id="2b083-126">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="2b083-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="2b083-127">応答</span><span class="sxs-lookup"><span data-stu-id="2b083-127">Response</span></span>

<span data-ttu-id="2b083-128">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b083-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="2b083-129">例</span><span class="sxs-lookup"><span data-stu-id="2b083-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b083-130">要求</span><span class="sxs-lookup"><span data-stu-id="2b083-130">Request</span></span>

<span data-ttu-id="2b083-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b083-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="2b083-132">応答</span><span class="sxs-lookup"><span data-stu-id="2b083-132">Response</span></span>

<span data-ttu-id="2b083-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2b083-133">Here is an example of the response.</span></span>

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
