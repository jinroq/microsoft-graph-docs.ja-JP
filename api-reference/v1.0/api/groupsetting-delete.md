---
title: グループ設定の削除
description: グループ設定を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d046d9d0fa3cf4871c7e0438d8b82c84b008fd8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276805"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="6c101-103">グループ設定の削除</span><span class="sxs-lookup"><span data-stu-id="6c101-103">Delete a group setting</span></span>

<span data-ttu-id="6c101-104">グループ設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c101-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c101-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c101-105">Permissions</span></span>

<span data-ttu-id="6c101-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6c101-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c101-108">Permission type</span></span>      | <span data-ttu-id="6c101-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c101-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c101-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c101-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c101-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c101-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c101-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c101-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c101-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c101-113">Not supported.</span></span>    |
|<span data-ttu-id="6c101-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c101-114">Application</span></span> | <span data-ttu-id="6c101-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c101-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c101-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c101-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="6c101-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c101-117">Request headers</span></span>

| <span data-ttu-id="6c101-118">名前</span><span class="sxs-lookup"><span data-stu-id="6c101-118">Name</span></span> | <span data-ttu-id="6c101-119">説明</span><span class="sxs-lookup"><span data-stu-id="6c101-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6c101-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c101-120">Authorization</span></span>  | <span data-ttu-id="6c101-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c101-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c101-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c101-123">Content-Type</span></span>  | <span data-ttu-id="6c101-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c101-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c101-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c101-125">Request body</span></span>
<span data-ttu-id="6c101-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6c101-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c101-127">応答</span><span class="sxs-lookup"><span data-stu-id="6c101-127">Response</span></span>

<span data-ttu-id="6c101-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6c101-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c101-130">例</span><span class="sxs-lookup"><span data-stu-id="6c101-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c101-131">要求</span><span class="sxs-lookup"><span data-stu-id="6c101-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="6c101-132">応答</span><span class="sxs-lookup"><span data-stu-id="6c101-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c101-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="6c101-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c101-134">C#</span><span class="sxs-lookup"><span data-stu-id="6c101-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c101-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c101-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_groupsetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c101-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="6c101-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_groupsetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/groupsetting-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
