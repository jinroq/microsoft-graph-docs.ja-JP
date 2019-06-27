---
title: 'TableColumn: TotalRowRange'
description: 列の集計行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f1eac8f83fe2c4ca27016038dcf1829dcbea53f5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270932"
---
# <a name="tablecolumn-totalrowrange"></a><span data-ttu-id="85210-103">TableColumn: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="85210-103">TableColumn: TotalRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85210-104">列の集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="85210-104">Gets the range object associated with the totals row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="85210-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="85210-105">Permissions</span></span>
<span data-ttu-id="85210-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85210-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85210-108">Permission type</span></span>      | <span data-ttu-id="85210-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="85210-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85210-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85210-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85210-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85210-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85210-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85210-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85210-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85210-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85210-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85210-114">Application</span></span> | <span data-ttu-id="85210-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85210-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85210-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85210-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/TotalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="85210-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85210-117">Request headers</span></span>
| <span data-ttu-id="85210-118">名前</span><span class="sxs-lookup"><span data-stu-id="85210-118">Name</span></span>       | <span data-ttu-id="85210-119">説明</span><span class="sxs-lookup"><span data-stu-id="85210-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85210-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="85210-120">Authorization</span></span>  | <span data-ttu-id="85210-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="85210-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85210-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85210-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="85210-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="85210-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85210-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="85210-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="85210-127">応答</span><span class="sxs-lookup"><span data-stu-id="85210-127">Response</span></span>

<span data-ttu-id="85210-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="85210-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85210-129">例</span><span class="sxs-lookup"><span data-stu-id="85210-129">Example</span></span>
<span data-ttu-id="85210-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="85210-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85210-131">要求</span><span class="sxs-lookup"><span data-stu-id="85210-131">Request</span></span>
<span data-ttu-id="85210-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85210-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_totalrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/TotalRowRange
```

##### <a name="response"></a><span data-ttu-id="85210-133">応答</span><span class="sxs-lookup"><span data-stu-id="85210-133">Response</span></span>
<span data-ttu-id="85210-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85210-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="85210-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="85210-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85210-138">C#</span><span class="sxs-lookup"><span data-stu-id="85210-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumn_totalrowrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85210-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="85210-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumn_totalrowrange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="85210-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="85210-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecolumn_totalrowrange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tablecolumn-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumn-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
