---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0921a946ce0b22a49a978530981184c06fbf84a3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260719"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="d4dc7-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="d4dc7-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4dc7-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4dc7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d4dc7-105">Permissions</span></span>

<span data-ttu-id="d4dc7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4dc7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4dc7-108">Permission type</span></span>      | <span data-ttu-id="d4dc7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4dc7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4dc7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4dc7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4dc7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4dc7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4dc7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4dc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4dc7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-113">Not supported.</span></span>    |
|<span data-ttu-id="d4dc7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4dc7-114">Application</span></span> | <span data-ttu-id="d4dc7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4dc7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4dc7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d4dc7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4dc7-117">Request headers</span></span>

| <span data-ttu-id="d4dc7-118">名前</span><span class="sxs-lookup"><span data-stu-id="d4dc7-118">Name</span></span>       | <span data-ttu-id="d4dc7-119">型</span><span class="sxs-lookup"><span data-stu-id="d4dc7-119">Type</span></span> | <span data-ttu-id="d4dc7-120">説明</span><span class="sxs-lookup"><span data-stu-id="d4dc7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d4dc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4dc7-121">Authorization</span></span>  | <span data-ttu-id="d4dc7-122">string</span><span class="sxs-lookup"><span data-stu-id="d4dc7-122">string</span></span>  | <span data-ttu-id="d4dc7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4dc7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4dc7-125">Request body</span></span>

<span data-ttu-id="d4dc7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4dc7-127">応答</span><span class="sxs-lookup"><span data-stu-id="d4dc7-127">Response</span></span>

<span data-ttu-id="d4dc7-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4dc7-130">例</span><span class="sxs-lookup"><span data-stu-id="d4dc7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4dc7-131">要求</span><span class="sxs-lookup"><span data-stu-id="d4dc7-131">Request</span></span>

<span data-ttu-id="d4dc7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="d4dc7-133">応答</span><span class="sxs-lookup"><span data-stu-id="d4dc7-133">Response</span></span>

<span data-ttu-id="d4dc7-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d4dc7-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4dc7-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d4dc7-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4dc7-136">C#</span><span class="sxs-lookup"><span data-stu-id="d4dc7-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4dc7-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4dc7-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d4dc7-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="d4dc7-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
