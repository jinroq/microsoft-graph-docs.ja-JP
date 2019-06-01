---
title: directoryObject を削除する
description: directoryObject を削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d550a12839bdb1bb6520edd35ef08e0322d8e2fe
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657015"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="7c58a-103">directoryObject を削除する</span><span class="sxs-lookup"><span data-stu-id="7c58a-103">Delete directoryObject</span></span>

<span data-ttu-id="7c58a-104">directoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="7c58a-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c58a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c58a-105">Permissions</span></span>
<span data-ttu-id="7c58a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c58a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c58a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c58a-108">Permission type</span></span>      | <span data-ttu-id="7c58a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c58a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c58a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c58a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c58a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c58a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c58a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c58a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c58a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c58a-113">Not supported.</span></span>    |
|<span data-ttu-id="7c58a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c58a-114">Application</span></span> | <span data-ttu-id="7c58a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c58a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c58a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c58a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7c58a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c58a-117">Request headers</span></span>
| <span data-ttu-id="7c58a-118">名前</span><span class="sxs-lookup"><span data-stu-id="7c58a-118">Name</span></span>       | <span data-ttu-id="7c58a-119">型</span><span class="sxs-lookup"><span data-stu-id="7c58a-119">Type</span></span> | <span data-ttu-id="7c58a-120">説明</span><span class="sxs-lookup"><span data-stu-id="7c58a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c58a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c58a-121">Authorization</span></span>  | <span data-ttu-id="7c58a-122">string</span><span class="sxs-lookup"><span data-stu-id="7c58a-122">string</span></span>  | <span data-ttu-id="7c58a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c58a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c58a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c58a-125">Request body</span></span>
<span data-ttu-id="7c58a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c58a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c58a-127">応答</span><span class="sxs-lookup"><span data-stu-id="7c58a-127">Response</span></span>

<span data-ttu-id="7c58a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7c58a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c58a-130">例</span><span class="sxs-lookup"><span data-stu-id="7c58a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c58a-131">要求</span><span class="sxs-lookup"><span data-stu-id="7c58a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="7c58a-132">応答</span><span class="sxs-lookup"><span data-stu-id="7c58a-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c58a-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7c58a-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c58a-134">C#</span><span class="sxs-lookup"><span data-stu-id="7c58a-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c58a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c58a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
