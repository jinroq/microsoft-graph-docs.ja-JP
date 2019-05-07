---
title: Delete groupLifecyclePolicy
description: groupLifecyclePolicy を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ae3d415f04803dd197a8da666612c65eed77be8b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613554"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="d0e0c-103">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d0e0c-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="d0e0c-104">[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0e0c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d0e0c-105">Permissions</span></span>

<span data-ttu-id="d0e0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0e0c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0e0c-108">Permission type</span></span>      | <span data-ttu-id="d0e0c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0e0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0e0c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0e0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0e0c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e0c-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0e0c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0e0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0e0c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-113">Not supported.</span></span>    |
|<span data-ttu-id="d0e0c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0e0c-114">Application</span></span> | <span data-ttu-id="d0e0c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e0c-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0e0c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0e0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="d0e0c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0e0c-117">Request headers</span></span>

| <span data-ttu-id="d0e0c-118">名前</span><span class="sxs-lookup"><span data-stu-id="d0e0c-118">Name</span></span> | <span data-ttu-id="d0e0c-119">説明</span><span class="sxs-lookup"><span data-stu-id="d0e0c-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d0e0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0e0c-120">Authorization</span></span> | <span data-ttu-id="d0e0c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0e0c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0e0c-123">Content-Type</span></span>  | <span data-ttu-id="d0e0c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0e0c-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0e0c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0e0c-125">Request body</span></span>
<span data-ttu-id="d0e0c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d0e0c-127">応答</span><span class="sxs-lookup"><span data-stu-id="d0e0c-127">Response</span></span>

<span data-ttu-id="d0e0c-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d0e0c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0e0c-130">例</span><span class="sxs-lookup"><span data-stu-id="d0e0c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d0e0c-131">要求</span><span class="sxs-lookup"><span data-stu-id="d0e0c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="d0e0c-132">応答</span><span class="sxs-lookup"><span data-stu-id="d0e0c-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0e0c-133">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d0e0c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0e0c-134">Visual</span><span class="sxs-lookup"><span data-stu-id="d0e0c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0e0c-135">Java</span><span class="sxs-lookup"><span data-stu-id="d0e0c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
