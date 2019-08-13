---
title: 範囲:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 239911c34978cd2fd8ee766fd318343a28057a8c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365119"
---
# <a name="range-cell"></a><span data-ttu-id="53270-105">範囲:セル</span><span class="sxs-lookup"><span data-stu-id="53270-105">Range: Cell</span></span>

<span data-ttu-id="53270-p102">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。</span><span class="sxs-lookup"><span data-stu-id="53270-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="53270-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53270-109">Permissions</span></span>
<span data-ttu-id="53270-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53270-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53270-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53270-112">Permission type</span></span>      | <span data-ttu-id="53270-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53270-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53270-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53270-114">Delegated (work or school account)</span></span> | <span data-ttu-id="53270-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53270-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53270-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53270-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53270-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53270-117">Not supported.</span></span>    |
|<span data-ttu-id="53270-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53270-118">Application</span></span> | <span data-ttu-id="53270-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53270-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53270-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53270-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="53270-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53270-121">Request headers</span></span>
| <span data-ttu-id="53270-122">名前</span><span class="sxs-lookup"><span data-stu-id="53270-122">Name</span></span>       | <span data-ttu-id="53270-123">説明</span><span class="sxs-lookup"><span data-stu-id="53270-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53270-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="53270-124">Authorization</span></span>  | <span data-ttu-id="53270-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53270-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53270-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53270-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="53270-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="53270-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="53270-130">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="53270-130">Path parameters</span></span>
<span data-ttu-id="53270-131">パスに、次のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="53270-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="53270-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="53270-132">Parameter</span></span>    | <span data-ttu-id="53270-133">型</span><span class="sxs-lookup"><span data-stu-id="53270-133">Type</span></span>   |<span data-ttu-id="53270-134">説明</span><span class="sxs-lookup"><span data-stu-id="53270-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53270-135">row</span><span class="sxs-lookup"><span data-stu-id="53270-135">row</span></span>|<span data-ttu-id="53270-136">Int32</span><span class="sxs-lookup"><span data-stu-id="53270-136">Int32</span></span>|<span data-ttu-id="53270-p106">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="53270-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="53270-139">column</span><span class="sxs-lookup"><span data-stu-id="53270-139">column</span></span>|<span data-ttu-id="53270-140">Int32</span><span class="sxs-lookup"><span data-stu-id="53270-140">Int32</span></span>|<span data-ttu-id="53270-p107">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="53270-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="53270-143">応答</span><span class="sxs-lookup"><span data-stu-id="53270-143">Response</span></span>

<span data-ttu-id="53270-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53270-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53270-145">例</span><span class="sxs-lookup"><span data-stu-id="53270-145">Example</span></span>
<span data-ttu-id="53270-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="53270-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53270-147">要求</span><span class="sxs-lookup"><span data-stu-id="53270-147">Request</span></span>
<span data-ttu-id="53270-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53270-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53270-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="53270-149">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53270-150">C#</span><span class="sxs-lookup"><span data-stu-id="53270-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53270-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53270-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53270-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="53270-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="53270-153">Java</span><span class="sxs-lookup"><span data-stu-id="53270-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-cell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53270-154">応答</span><span class="sxs-lookup"><span data-stu-id="53270-154">Response</span></span>
<span data-ttu-id="53270-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53270-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
