---
title: 'Chart: setData'
description: グラフのソース データをリセットします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b028ca325d4f047e7b13b46fa1edd33385827457
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272626"
---
# <a name="chart-setdata"></a><span data-ttu-id="8c605-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="8c605-103">Chart: setData</span></span>

<span data-ttu-id="8c605-104">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="8c605-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c605-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8c605-105">Permissions</span></span>
<span data-ttu-id="8c605-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c605-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c605-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c605-108">Permission type</span></span>      | <span data-ttu-id="8c605-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c605-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c605-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c605-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c605-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c605-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c605-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c605-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c605-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c605-113">Not supported.</span></span>    |
|<span data-ttu-id="8c605-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c605-114">Application</span></span> | <span data-ttu-id="8c605-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c605-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c605-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c605-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="8c605-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c605-117">Request headers</span></span>
| <span data-ttu-id="8c605-118">名前</span><span class="sxs-lookup"><span data-stu-id="8c605-118">Name</span></span>       | <span data-ttu-id="8c605-119">説明</span><span class="sxs-lookup"><span data-stu-id="8c605-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c605-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c605-120">Authorization</span></span>  | <span data-ttu-id="8c605-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8c605-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c605-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c605-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c605-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8c605-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c605-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c605-126">Request body</span></span>
<span data-ttu-id="8c605-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8c605-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c605-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8c605-128">Parameter</span></span>    | <span data-ttu-id="8c605-129">型</span><span class="sxs-lookup"><span data-stu-id="8c605-129">Type</span></span>   |<span data-ttu-id="8c605-130">説明</span><span class="sxs-lookup"><span data-stu-id="8c605-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c605-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="8c605-131">sourceData</span></span>|<span data-ttu-id="8c605-132">Json</span><span class="sxs-lookup"><span data-stu-id="8c605-132">Json</span></span>|<span data-ttu-id="8c605-133">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8c605-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="8c605-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="8c605-134">seriesBy</span></span>|<span data-ttu-id="8c605-135">string</span><span class="sxs-lookup"><span data-stu-id="8c605-135">string</span></span>|<span data-ttu-id="8c605-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8c605-136">Optional.</span></span> <span data-ttu-id="8c605-137">列や行がグラフのデータ系列として使用される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c605-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="8c605-138">Auto (既定)、行、列のいずれかをすることができます。</span><span class="sxs-lookup"><span data-stu-id="8c605-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="8c605-139">使用可能な値: `Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="8c605-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="8c605-140">応答</span><span class="sxs-lookup"><span data-stu-id="8c605-140">Response</span></span>

<span data-ttu-id="8c605-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8c605-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c605-143">例</span><span class="sxs-lookup"><span data-stu-id="8c605-143">Example</span></span>
<span data-ttu-id="8c605-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8c605-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c605-145">要求</span><span class="sxs-lookup"><span data-stu-id="8c605-145">Request</span></span>
<span data-ttu-id="8c605-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c605-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="8c605-147">応答</span><span class="sxs-lookup"><span data-stu-id="8c605-147">Response</span></span>
<span data-ttu-id="8c605-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8c605-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c605-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="8c605-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c605-150">C#</span><span class="sxs-lookup"><span data-stu-id="8c605-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setdata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c605-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c605-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setdata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8c605-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="8c605-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setdata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
