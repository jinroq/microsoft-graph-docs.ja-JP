---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
ms.openlocfilehash: a4b32e00719772f6dcfb715fa69350edf9a8b48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021102"
---
# <a name="delete-an-activity"></a><span data-ttu-id="eb126-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="eb126-103">Delete an activity</span></span>

<span data-ttu-id="eb126-104">アプリの既存のユーザーのアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="eb126-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb126-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb126-105">Permissions</span></span>

<span data-ttu-id="eb126-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eb126-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb126-108">Permission type</span></span>      | <span data-ttu-id="eb126-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb126-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb126-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb126-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb126-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="eb126-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="eb126-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb126-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb126-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="eb126-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="eb126-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb126-114">Application</span></span> | <span data-ttu-id="eb126-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb126-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb126-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb126-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb126-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb126-117">Request headers</span></span>

|<span data-ttu-id="eb126-118">名前</span><span class="sxs-lookup"><span data-stu-id="eb126-118">Name</span></span> | <span data-ttu-id="eb126-119">型</span><span class="sxs-lookup"><span data-stu-id="eb126-119">Type</span></span> | <span data-ttu-id="eb126-120">説明</span><span class="sxs-lookup"><span data-stu-id="eb126-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="eb126-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb126-121">Authorization</span></span> | <span data-ttu-id="eb126-122">string</span><span class="sxs-lookup"><span data-stu-id="eb126-122">string</span></span> | <span data-ttu-id="eb126-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eb126-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb126-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb126-125">Request body</span></span>

<span data-ttu-id="eb126-126">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="eb126-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="eb126-127">応答</span><span class="sxs-lookup"><span data-stu-id="eb126-127">Response</span></span>

<span data-ttu-id="eb126-128">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="eb126-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="eb126-129">例</span><span class="sxs-lookup"><span data-stu-id="eb126-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb126-130">要求</span><span class="sxs-lookup"><span data-stu-id="eb126-130">Request</span></span>

<span data-ttu-id="eb126-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb126-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="eb126-132">応答</span><span class="sxs-lookup"><span data-stu-id="eb126-132">Response</span></span>

<span data-ttu-id="eb126-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eb126-133">Here is an example of the response.</span></span>

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