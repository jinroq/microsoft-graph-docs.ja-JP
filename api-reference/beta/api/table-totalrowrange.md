---
title: Table:TotalRowRange
description: テーブルの集計行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16ec7f98343587ba48ba08d2f82da6ffe1dfde3f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271037"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="377aa-103">Table:TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="377aa-103">Table: TotalRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="377aa-104">テーブルの集計行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="377aa-104">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="377aa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="377aa-105">Permissions</span></span>
<span data-ttu-id="377aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="377aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="377aa-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="377aa-108">Permission type</span></span>      | <span data-ttu-id="377aa-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="377aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="377aa-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="377aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="377aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="377aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="377aa-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="377aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="377aa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="377aa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="377aa-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="377aa-114">Application</span></span> | <span data-ttu-id="377aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="377aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="377aa-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="377aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/TotalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="377aa-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="377aa-117">Request headers</span></span>
| <span data-ttu-id="377aa-118">名前</span><span class="sxs-lookup"><span data-stu-id="377aa-118">Name</span></span>       | <span data-ttu-id="377aa-119">説明</span><span class="sxs-lookup"><span data-stu-id="377aa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="377aa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="377aa-120">Authorization</span></span>  | <span data-ttu-id="377aa-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="377aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="377aa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="377aa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="377aa-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="377aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="377aa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="377aa-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="377aa-127">応答</span><span class="sxs-lookup"><span data-stu-id="377aa-127">Response</span></span>

<span data-ttu-id="377aa-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="377aa-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="377aa-129">例</span><span class="sxs-lookup"><span data-stu-id="377aa-129">Example</span></span>
<span data-ttu-id="377aa-130">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="377aa-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="377aa-131">要求</span><span class="sxs-lookup"><span data-stu-id="377aa-131">Request</span></span>
<span data-ttu-id="377aa-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="377aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_totalrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange
```

##### <a name="response"></a><span data-ttu-id="377aa-133">応答</span><span class="sxs-lookup"><span data-stu-id="377aa-133">Response</span></span>
<span data-ttu-id="377aa-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="377aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="377aa-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="377aa-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="377aa-138">C#</span><span class="sxs-lookup"><span data-stu-id="377aa-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/table_totalrowrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="377aa-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="377aa-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/table_totalrowrange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="377aa-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="377aa-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/table_totalrowrange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/table-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-totalrowrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
