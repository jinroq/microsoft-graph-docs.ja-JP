---
title: 所有者の削除
description: この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: dc0f9d7aea0d718cf4c467fa789ec42aa6f2ee7b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263312"
---
# <a name="remove-owner"></a><span data-ttu-id="db42c-103">所有者の削除</span><span class="sxs-lookup"><span data-stu-id="db42c-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db42c-104">この API を使用して、owners ナビゲーション プロパティを通じて Office 365 のグループ、セキュリティ グループ、メールが有効なセキュリティ グループから所有者を削除できます。</span><span class="sxs-lookup"><span data-stu-id="db42c-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="db42c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db42c-105">Permissions</span></span>
<span data-ttu-id="db42c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db42c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db42c-108">Permission type</span></span>      | <span data-ttu-id="db42c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db42c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db42c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db42c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db42c-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db42c-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db42c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db42c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db42c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db42c-113">Not supported.</span></span>    |
|<span data-ttu-id="db42c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db42c-114">Application</span></span> | <span data-ttu-id="db42c-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db42c-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db42c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db42c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="db42c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db42c-117">Request headers</span></span>
| <span data-ttu-id="db42c-118">名前</span><span class="sxs-lookup"><span data-stu-id="db42c-118">Name</span></span>       | <span data-ttu-id="db42c-119">型</span><span class="sxs-lookup"><span data-stu-id="db42c-119">Type</span></span> | <span data-ttu-id="db42c-120">説明</span><span class="sxs-lookup"><span data-stu-id="db42c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db42c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db42c-121">Authorization</span></span>  | <span data-ttu-id="db42c-122">string</span><span class="sxs-lookup"><span data-stu-id="db42c-122">string</span></span>  | <span data-ttu-id="db42c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db42c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db42c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="db42c-125">Request body</span></span>
<span data-ttu-id="db42c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="db42c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db42c-127">応答</span><span class="sxs-lookup"><span data-stu-id="db42c-127">Response</span></span>
<span data-ttu-id="db42c-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="db42c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db42c-130">例</span><span class="sxs-lookup"><span data-stu-id="db42c-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="db42c-131">要求</span><span class="sxs-lookup"><span data-stu-id="db42c-131">Request</span></span>
<span data-ttu-id="db42c-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="db42c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="db42c-133">要求内で、$ref セグメント後に削除したいディレクトリ オブジェクトの `id` を指定します。</span><span class="sxs-lookup"><span data-stu-id="db42c-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="db42c-134">応答</span><span class="sxs-lookup"><span data-stu-id="db42c-134">Response</span></span>
<span data-ttu-id="db42c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="db42c-135">The following is an example of the response.</span></span>
><span data-ttu-id="db42c-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="db42c-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db42c-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="db42c-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="db42c-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="db42c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="db42c-139">C#</span><span class="sxs-lookup"><span data-stu-id="db42c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db42c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="db42c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="db42c-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="db42c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
