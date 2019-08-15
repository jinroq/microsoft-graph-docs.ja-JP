---
title: Delete groupLifecyclePolicy
description: groupLifecyclePolicy を削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: df6044ed4e75ca60fe01873af36d4220a299564c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420559"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="4adf8-103">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="4adf8-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4adf8-104">[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4adf8-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4adf8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4adf8-105">Permissions</span></span>

<span data-ttu-id="4adf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4adf8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4adf8-108">Permission type</span></span>      | <span data-ttu-id="4adf8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4adf8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4adf8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4adf8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4adf8-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4adf8-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4adf8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4adf8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4adf8-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="4adf8-113">Not supported</span></span> |
|<span data-ttu-id="4adf8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4adf8-114">Application</span></span> | <span data-ttu-id="4adf8-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4adf8-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4adf8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4adf8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="4adf8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4adf8-117">Request headers</span></span>

| <span data-ttu-id="4adf8-118">名前</span><span class="sxs-lookup"><span data-stu-id="4adf8-118">Name</span></span> | <span data-ttu-id="4adf8-119">説明</span><span class="sxs-lookup"><span data-stu-id="4adf8-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4adf8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4adf8-120">Authorization</span></span> | <span data-ttu-id="4adf8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4adf8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4adf8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4adf8-123">Content-Type</span></span>  | <span data-ttu-id="4adf8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4adf8-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4adf8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4adf8-125">Request body</span></span>
<span data-ttu-id="4adf8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4adf8-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4adf8-127">応答</span><span class="sxs-lookup"><span data-stu-id="4adf8-127">Response</span></span>

<span data-ttu-id="4adf8-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4adf8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4adf8-130">例</span><span class="sxs-lookup"><span data-stu-id="4adf8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4adf8-131">要求</span><span class="sxs-lookup"><span data-stu-id="4adf8-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4adf8-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4adf8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4adf8-133">C#</span><span class="sxs-lookup"><span data-stu-id="4adf8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4adf8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4adf8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4adf8-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="4adf8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4adf8-136">応答</span><span class="sxs-lookup"><span data-stu-id="4adf8-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
