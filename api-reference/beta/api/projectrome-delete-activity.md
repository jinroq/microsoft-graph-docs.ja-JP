---
title: アクティビティを削除する
description: アプリの既存のユーザーアクティビティを削除します。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: bfe143e4f3532b9b85ebea587cb8858081d1182f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988511"
---
# <a name="delete-an-activity"></a><span data-ttu-id="1b970-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="1b970-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b970-104">アプリの既存のユーザーアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="1b970-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b970-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1b970-105">Permissions</span></span>

<span data-ttu-id="1b970-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1b970-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b970-108">Permission type</span></span>      | <span data-ttu-id="1b970-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b970-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b970-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b970-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b970-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1b970-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1b970-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b970-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b970-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1b970-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1b970-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b970-114">Application</span></span> | <span data-ttu-id="1b970-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b970-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b970-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b970-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b970-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b970-117">Request headers</span></span>

|<span data-ttu-id="1b970-118">名前</span><span class="sxs-lookup"><span data-stu-id="1b970-118">Name</span></span> | <span data-ttu-id="1b970-119">型</span><span class="sxs-lookup"><span data-stu-id="1b970-119">Type</span></span> | <span data-ttu-id="1b970-120">説明</span><span class="sxs-lookup"><span data-stu-id="1b970-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1b970-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b970-121">Authorization</span></span> | <span data-ttu-id="1b970-122">string</span><span class="sxs-lookup"><span data-stu-id="1b970-122">string</span></span> | <span data-ttu-id="1b970-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1b970-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b970-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b970-125">Request body</span></span>

<span data-ttu-id="1b970-126">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="1b970-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1b970-127">応答</span><span class="sxs-lookup"><span data-stu-id="1b970-127">Response</span></span>

<span data-ttu-id="1b970-128">成功した場合、このメソッド`204 No Content`は、アクティビティが削除された場合に応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1b970-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="1b970-129">例</span><span class="sxs-lookup"><span data-stu-id="1b970-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b970-130">要求</span><span class="sxs-lookup"><span data-stu-id="1b970-130">Request</span></span>

<span data-ttu-id="1b970-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b970-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1b970-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1b970-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b970-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b970-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b970-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b970-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b970-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="1b970-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1b970-136">Java</span><span class="sxs-lookup"><span data-stu-id="1b970-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b970-137">応答</span><span class="sxs-lookup"><span data-stu-id="1b970-137">Response</span></span>

<span data-ttu-id="1b970-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1b970-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
