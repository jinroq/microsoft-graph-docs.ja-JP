---
title: AccessReview の削除
description: Azure AD access レビュー機能で、accessReview オブジェクトを削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d7a7434d4de008ce2a3f597636c30fcf014f3de8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258983"
---
# <a name="delete-accessreview"></a><span data-ttu-id="0e9e5-103">AccessReview の削除</span><span class="sxs-lookup"><span data-stu-id="0e9e5-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e9e5-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e9e5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e9e5-105">Permissions</span></span>
<span data-ttu-id="0e9e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e9e5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e9e5-108">Permission type</span></span>                        | <span data-ttu-id="0e9e5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e9e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e9e5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e9e5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e9e5-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e9e5-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0e9e5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e9e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e9e5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-113">Not supported.</span></span> |
|<span data-ttu-id="0e9e5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e9e5-114">Application</span></span>                            | <span data-ttu-id="0e9e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-115">Not supported.</span></span> |

<span data-ttu-id="0e9e5-116">また、呼び出し元には、 [programcontrol](../resources/programcontrol.md)を削除できるように、すべてのアクセス許可が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="0e9e5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e9e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="0e9e5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e9e5-118">Request headers</span></span>
| <span data-ttu-id="0e9e5-119">名前</span><span class="sxs-lookup"><span data-stu-id="0e9e5-119">Name</span></span>         | <span data-ttu-id="0e9e5-120">型</span><span class="sxs-lookup"><span data-stu-id="0e9e5-120">Type</span></span>        | <span data-ttu-id="0e9e5-121">説明</span><span class="sxs-lookup"><span data-stu-id="0e9e5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0e9e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e9e5-122">Authorization</span></span> | <span data-ttu-id="0e9e5-123">string</span><span class="sxs-lookup"><span data-stu-id="0e9e5-123">string</span></span> | <span data-ttu-id="0e9e5-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e9e5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e9e5-126">Request body</span></span>
<span data-ttu-id="0e9e5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0e9e5-128">応答</span><span class="sxs-lookup"><span data-stu-id="0e9e5-128">Response</span></span>
<span data-ttu-id="0e9e5-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e9e5-131">例</span><span class="sxs-lookup"><span data-stu-id="0e9e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e9e5-132">要求</span><span class="sxs-lookup"><span data-stu-id="0e9e5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
##### <a name="response"></a><span data-ttu-id="0e9e5-133">応答</span><span class="sxs-lookup"><span data-stu-id="0e9e5-133">Response</span></span>
><span data-ttu-id="0e9e5-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0e9e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0e9e5-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0e9e5-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0e9e5-137">C#</span><span class="sxs-lookup"><span data-stu-id="0e9e5-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e9e5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e9e5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e9e5-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e9e5-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
