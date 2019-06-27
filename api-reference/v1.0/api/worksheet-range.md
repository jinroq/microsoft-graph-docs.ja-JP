---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a5e1d2ba70e5cdb5ca1e38e4baba0ddf9977fc9c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278310"
---
# <a name="worksheet-range"></a><span data-ttu-id="7a864-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="7a864-103">Worksheet: Range</span></span>

<span data-ttu-id="7a864-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="7a864-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a864-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7a864-105">Permissions</span></span>
<span data-ttu-id="7a864-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a864-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a864-108">Permission type</span></span>      | <span data-ttu-id="7a864-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a864-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a864-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a864-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a864-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a864-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a864-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a864-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a864-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a864-113">Not supported.</span></span>    |
|<span data-ttu-id="7a864-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a864-114">Application</span></span> | <span data-ttu-id="7a864-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a864-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a864-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a864-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="7a864-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a864-117">Request headers</span></span>
| <span data-ttu-id="7a864-118">名前</span><span class="sxs-lookup"><span data-stu-id="7a864-118">Name</span></span>       | <span data-ttu-id="7a864-119">説明</span><span class="sxs-lookup"><span data-stu-id="7a864-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a864-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a864-120">Authorization</span></span>  | <span data-ttu-id="7a864-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7a864-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a864-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7a864-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7a864-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7a864-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="7a864-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="7a864-126">Function parameters</span></span>

| <span data-ttu-id="7a864-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7a864-127">Parameter</span></span>    | <span data-ttu-id="7a864-128">型</span><span class="sxs-lookup"><span data-stu-id="7a864-128">Type</span></span>   |<span data-ttu-id="7a864-129">説明</span><span class="sxs-lookup"><span data-stu-id="7a864-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a864-130">address</span><span class="sxs-lookup"><span data-stu-id="7a864-130">address</span></span>|<span data-ttu-id="7a864-131">string</span><span class="sxs-lookup"><span data-stu-id="7a864-131">string</span></span>|<span data-ttu-id="7a864-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="7a864-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="7a864-135">応答</span><span class="sxs-lookup"><span data-stu-id="7a864-135">Response</span></span>

<span data-ttu-id="7a864-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7a864-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a864-137">例</span><span class="sxs-lookup"><span data-stu-id="7a864-137">Example</span></span>
<span data-ttu-id="7a864-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7a864-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7a864-139">要求</span><span class="sxs-lookup"><span data-stu-id="7a864-139">Request</span></span>
<span data-ttu-id="7a864-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a864-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="7a864-141">応答</span><span class="sxs-lookup"><span data-stu-id="7a864-141">Response</span></span>
<span data-ttu-id="7a864-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a864-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7a864-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7a864-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7a864-146">C#</span><span class="sxs-lookup"><span data-stu-id="7a864-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a864-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a864-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7a864-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="7a864-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_range-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="7a864-149">オプション`address`のパラメーターが指定されていない場合、この関数はワークシートの範囲全体を返します。</span><span class="sxs-lookup"><span data-stu-id="7a864-149">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="7a864-150">要求</span><span class="sxs-lookup"><span data-stu-id="7a864-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="7a864-151">応答</span><span class="sxs-lookup"><span data-stu-id="7a864-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7a864-152">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7a864-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7a864-153">C#</span><span class="sxs-lookup"><span data-stu-id="7a864-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a864-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a864-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7a864-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="7a864-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_range_noaddress-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
