---
title: 履歴項目を削除する
description: 既存のユーザーアクティビティの既存の履歴項目を削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5a3cac83c220a8fa15a3d5277af319117bd7c927
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264065"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="94052-103">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="94052-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94052-104">既存のユーザーアクティビティの既存の履歴項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="94052-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="94052-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94052-105">Permissions</span></span>

<span data-ttu-id="94052-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94052-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94052-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94052-108">Permission type</span></span>      | <span data-ttu-id="94052-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94052-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94052-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94052-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94052-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="94052-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="94052-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94052-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94052-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="94052-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="94052-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94052-114">Application</span></span> | <span data-ttu-id="94052-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94052-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94052-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94052-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94052-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94052-117">Request headers</span></span>

|<span data-ttu-id="94052-118">名前</span><span class="sxs-lookup"><span data-stu-id="94052-118">Name</span></span> | <span data-ttu-id="94052-119">型</span><span class="sxs-lookup"><span data-stu-id="94052-119">Type</span></span> | <span data-ttu-id="94052-120">説明</span><span class="sxs-lookup"><span data-stu-id="94052-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="94052-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94052-121">Authorization</span></span> | <span data-ttu-id="94052-122">string</span><span class="sxs-lookup"><span data-stu-id="94052-122">string</span></span> | <span data-ttu-id="94052-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94052-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94052-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="94052-125">Request body</span></span>

<span data-ttu-id="94052-126">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="94052-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="94052-127">応答</span><span class="sxs-lookup"><span data-stu-id="94052-127">Response</span></span>

<span data-ttu-id="94052-128">成功した場合、このメソッド`204 No Content`は、履歴項目が削除された場合に応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="94052-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="94052-129">例</span><span class="sxs-lookup"><span data-stu-id="94052-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="94052-130">要求</span><span class="sxs-lookup"><span data-stu-id="94052-130">Request</span></span>

<span data-ttu-id="94052-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94052-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="94052-132">応答</span><span class="sxs-lookup"><span data-stu-id="94052-132">Response</span></span>

<span data-ttu-id="94052-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="94052-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="94052-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="94052-134">SDK sample code</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="94052-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="94052-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_historyItem-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)"
  ]
}
-->
