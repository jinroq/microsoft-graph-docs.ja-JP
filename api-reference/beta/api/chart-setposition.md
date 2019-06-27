---
title: 'Chart: setPosition'
description: ワークシート上のセルを基準にしてグラフを配置します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1baff92660d445c8c2d578db6a5b0ee63b863ca8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261923"
---
# <a name="chart-setposition"></a><span data-ttu-id="26756-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="26756-103">Chart: setPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26756-104">ワークシート上のセルを基準にしてグラフを配置します。</span><span class="sxs-lookup"><span data-stu-id="26756-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="26756-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26756-105">Permissions</span></span>
<span data-ttu-id="26756-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26756-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26756-108">Permission type</span></span>      | <span data-ttu-id="26756-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26756-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26756-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26756-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26756-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26756-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26756-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26756-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26756-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26756-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26756-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26756-114">Application</span></span> | <span data-ttu-id="26756-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26756-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26756-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26756-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="26756-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26756-117">Request headers</span></span>
| <span data-ttu-id="26756-118">名前</span><span class="sxs-lookup"><span data-stu-id="26756-118">Name</span></span>       | <span data-ttu-id="26756-119">説明</span><span class="sxs-lookup"><span data-stu-id="26756-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26756-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="26756-120">Authorization</span></span>  | <span data-ttu-id="26756-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26756-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26756-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="26756-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="26756-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="26756-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26756-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="26756-126">Request body</span></span>
<span data-ttu-id="26756-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="26756-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26756-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="26756-128">Parameter</span></span>    | <span data-ttu-id="26756-129">型</span><span class="sxs-lookup"><span data-stu-id="26756-129">Type</span></span>   |<span data-ttu-id="26756-130">説明</span><span class="sxs-lookup"><span data-stu-id="26756-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26756-131">startCell</span><span class="sxs-lookup"><span data-stu-id="26756-131">startCell</span></span>|<span data-ttu-id="26756-132">string</span><span class="sxs-lookup"><span data-stu-id="26756-132">string</span></span>|<span data-ttu-id="26756-p104">開始セル。これは、グラフの移動先です。開始セルは、ユーザーの右から左への表示の設定に応じて、左上のセルか、右上のセルとなります。</span><span class="sxs-lookup"><span data-stu-id="26756-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="26756-136">endCell</span><span class="sxs-lookup"><span data-stu-id="26756-136">endCell</span></span>|<span data-ttu-id="26756-137">string</span><span class="sxs-lookup"><span data-stu-id="26756-137">string</span></span>|<span data-ttu-id="26756-p105">省略可能。終了セル。指定されている場合、グラフの幅と高さは、このセルまたは範囲を完全にカバーするように設定されます。</span><span class="sxs-lookup"><span data-stu-id="26756-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="26756-141">応答</span><span class="sxs-lookup"><span data-stu-id="26756-141">Response</span></span>

<span data-ttu-id="26756-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="26756-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26756-144">例</span><span class="sxs-lookup"><span data-stu-id="26756-144">Example</span></span>
<span data-ttu-id="26756-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="26756-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26756-146">要求</span><span class="sxs-lookup"><span data-stu-id="26756-146">Request</span></span>
<span data-ttu-id="26756-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26756-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="26756-148">応答</span><span class="sxs-lookup"><span data-stu-id="26756-148">Response</span></span>
<span data-ttu-id="26756-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="26756-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="26756-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="26756-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="26756-151">C#</span><span class="sxs-lookup"><span data-stu-id="26756-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setposition-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26756-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="26756-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setposition-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="26756-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="26756-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setposition-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
