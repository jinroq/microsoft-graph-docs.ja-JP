---
title: 'RangeFormat: autofitRows'
description: 現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 26dd606524bff499d586bbc44ebc77fbf74692d7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274061"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="52fdf-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="52fdf-103">RangeFormat: autofitRows</span></span>

<span data-ttu-id="52fdf-104">現在の列のデータに基づいて、現在の範囲の行の高さを最適な高さに変更します。</span><span class="sxs-lookup"><span data-stu-id="52fdf-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="52fdf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52fdf-105">Permissions</span></span>
<span data-ttu-id="52fdf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52fdf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52fdf-108">Permission type</span></span>      | <span data-ttu-id="52fdf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52fdf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52fdf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52fdf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52fdf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52fdf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52fdf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52fdf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52fdf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52fdf-113">Not supported.</span></span>    |
|<span data-ttu-id="52fdf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52fdf-114">Application</span></span> | <span data-ttu-id="52fdf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52fdf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52fdf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52fdf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="52fdf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52fdf-117">Request headers</span></span>
| <span data-ttu-id="52fdf-118">名前</span><span class="sxs-lookup"><span data-stu-id="52fdf-118">Name</span></span>       | <span data-ttu-id="52fdf-119">説明</span><span class="sxs-lookup"><span data-stu-id="52fdf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52fdf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52fdf-120">Authorization</span></span>  | <span data-ttu-id="52fdf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52fdf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52fdf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52fdf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="52fdf-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="52fdf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52fdf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52fdf-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="52fdf-127">応答</span><span class="sxs-lookup"><span data-stu-id="52fdf-127">Response</span></span>

<span data-ttu-id="52fdf-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="52fdf-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52fdf-130">例</span><span class="sxs-lookup"><span data-stu-id="52fdf-130">Example</span></span>
<span data-ttu-id="52fdf-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="52fdf-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52fdf-132">要求</span><span class="sxs-lookup"><span data-stu-id="52fdf-132">Request</span></span>
<span data-ttu-id="52fdf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52fdf-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="52fdf-134">応答</span><span class="sxs-lookup"><span data-stu-id="52fdf-134">Response</span></span>
<span data-ttu-id="52fdf-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="52fdf-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52fdf-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="52fdf-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52fdf-137">C#</span><span class="sxs-lookup"><span data-stu-id="52fdf-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52fdf-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="52fdf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52fdf-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="52fdf-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangeformat_autofitrows-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeformat-autofitrows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
