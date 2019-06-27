---
title: 'ChartFill: clear'
description: グラフ要素の塗りつぶしの色をクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 01fa603e29a4d19e047bb0dd4cec92624255ab0b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272514"
---
# <a name="chartfill-clear"></a><span data-ttu-id="38f5a-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="38f5a-103">ChartFill: clear</span></span>

<span data-ttu-id="38f5a-104">グラフ要素の塗りつぶしの色をクリアします。</span><span class="sxs-lookup"><span data-stu-id="38f5a-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="38f5a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="38f5a-105">Permissions</span></span>
<span data-ttu-id="38f5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f5a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38f5a-108">Permission type</span></span>      | <span data-ttu-id="38f5a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="38f5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38f5a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38f5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38f5a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38f5a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="38f5a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38f5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38f5a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38f5a-113">Not supported.</span></span>    |
|<span data-ttu-id="38f5a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38f5a-114">Application</span></span> | <span data-ttu-id="38f5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38f5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38f5a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38f5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="38f5a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38f5a-117">Request headers</span></span>
| <span data-ttu-id="38f5a-118">名前</span><span class="sxs-lookup"><span data-stu-id="38f5a-118">Name</span></span>       | <span data-ttu-id="38f5a-119">説明</span><span class="sxs-lookup"><span data-stu-id="38f5a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38f5a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f5a-120">Authorization</span></span>  | <span data-ttu-id="38f5a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="38f5a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38f5a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="38f5a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="38f5a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="38f5a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f5a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="38f5a-126">Request body</span></span>
<span data-ttu-id="38f5a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="38f5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38f5a-128">応答</span><span class="sxs-lookup"><span data-stu-id="38f5a-128">Response</span></span>

<span data-ttu-id="38f5a-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="38f5a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f5a-131">例</span><span class="sxs-lookup"><span data-stu-id="38f5a-131">Example</span></span>
<span data-ttu-id="38f5a-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="38f5a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38f5a-133">要求</span><span class="sxs-lookup"><span data-stu-id="38f5a-133">Request</span></span>
<span data-ttu-id="38f5a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38f5a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="38f5a-135">応答</span><span class="sxs-lookup"><span data-stu-id="38f5a-135">Response</span></span>
<span data-ttu-id="38f5a-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="38f5a-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38f5a-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="38f5a-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38f5a-138">C#</span><span class="sxs-lookup"><span data-stu-id="38f5a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartfill_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38f5a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="38f5a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartfill_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38f5a-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="38f5a-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chartfill_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
