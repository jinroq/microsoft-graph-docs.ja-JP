---
title: 契約を削除する
description: アグリーメントオブジェクトを削除します。
localization_priority: Normal
ms.openlocfilehash: 1f6977ab76929b747330642c7d47dc427c231958
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258626"
---
# <a name="delete-agreement"></a><span data-ttu-id="0c039-103">契約を削除する</span><span class="sxs-lookup"><span data-stu-id="0c039-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c039-104">[アグリーメント](../resources/agreement.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="0c039-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c039-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0c039-105">Permissions</span></span>
<span data-ttu-id="0c039-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c039-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c039-108">Permission type</span></span>                        | <span data-ttu-id="0c039-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c039-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c039-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c039-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c039-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c039-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="0c039-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c039-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c039-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c039-113">Not supported.</span></span> |
|<span data-ttu-id="0c039-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c039-114">Application</span></span>                            | <span data-ttu-id="0c039-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c039-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c039-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c039-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="0c039-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c039-117">Request headers</span></span>
| <span data-ttu-id="0c039-118">名前</span><span class="sxs-lookup"><span data-stu-id="0c039-118">Name</span></span>         | <span data-ttu-id="0c039-119">型</span><span class="sxs-lookup"><span data-stu-id="0c039-119">Type</span></span>        | <span data-ttu-id="0c039-120">説明</span><span class="sxs-lookup"><span data-stu-id="0c039-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0c039-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c039-121">Authorization</span></span> | <span data-ttu-id="0c039-122">string</span><span class="sxs-lookup"><span data-stu-id="0c039-122">string</span></span> | <span data-ttu-id="0c039-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="0c039-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c039-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c039-125">Request body</span></span>
<span data-ttu-id="0c039-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0c039-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0c039-127">応答</span><span class="sxs-lookup"><span data-stu-id="0c039-127">Response</span></span>
<span data-ttu-id="0c039-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0c039-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c039-130">例</span><span class="sxs-lookup"><span data-stu-id="0c039-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c039-131">要求</span><span class="sxs-lookup"><span data-stu-id="0c039-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="0c039-132">応答</span><span class="sxs-lookup"><span data-stu-id="0c039-132">Response</span></span>
><span data-ttu-id="0c039-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0c039-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c039-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0c039-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c039-136">C#</span><span class="sxs-lookup"><span data-stu-id="0c039-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c039-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c039-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_agreement-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0c039-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="0c039-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_agreement-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
