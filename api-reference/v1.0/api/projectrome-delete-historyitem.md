---
title: 履歴項目を削除する
description: 既存のユーザーアクティビティの既存の履歴項目を削除します。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 39bb298d85d698de8548cbeeedf066c43122698c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025415"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="25a68-103">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="25a68-103">Delete a historyItem</span></span>

<span data-ttu-id="25a68-104">既存のユーザーアクティビティの既存の履歴項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="25a68-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="25a68-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="25a68-105">Permissions</span></span>

<span data-ttu-id="25a68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="25a68-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="25a68-108">Permission type</span></span>      | <span data-ttu-id="25a68-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="25a68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25a68-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="25a68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25a68-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="25a68-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="25a68-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="25a68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25a68-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="25a68-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="25a68-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="25a68-114">Application</span></span> | <span data-ttu-id="25a68-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25a68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25a68-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="25a68-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25a68-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="25a68-117">Request headers</span></span>

|<span data-ttu-id="25a68-118">名前</span><span class="sxs-lookup"><span data-stu-id="25a68-118">Name</span></span> | <span data-ttu-id="25a68-119">型</span><span class="sxs-lookup"><span data-stu-id="25a68-119">Type</span></span> | <span data-ttu-id="25a68-120">説明</span><span class="sxs-lookup"><span data-stu-id="25a68-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="25a68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25a68-121">Authorization</span></span> | <span data-ttu-id="25a68-122">string</span><span class="sxs-lookup"><span data-stu-id="25a68-122">string</span></span> | <span data-ttu-id="25a68-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="25a68-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25a68-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="25a68-125">Request body</span></span>

<span data-ttu-id="25a68-126">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="25a68-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="25a68-127">応答</span><span class="sxs-lookup"><span data-stu-id="25a68-127">Response</span></span>

<span data-ttu-id="25a68-128">成功した場合、このメソッド`204 No Content`は、履歴項目が削除された場合に応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="25a68-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="25a68-129">例</span><span class="sxs-lookup"><span data-stu-id="25a68-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25a68-130">要求</span><span class="sxs-lookup"><span data-stu-id="25a68-130">Request</span></span>

<span data-ttu-id="25a68-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="25a68-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="25a68-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="25a68-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="25a68-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="25a68-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25a68-134">応答</span><span class="sxs-lookup"><span data-stu-id="25a68-134">Response</span></span>

<span data-ttu-id="25a68-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="25a68-135">Here is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
