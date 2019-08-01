---
title: 範囲を更新する
description: 範囲オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4a7a29c429eb7240e13dedfd844d4e1af841e892
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022167"
---
# <a name="update-range"></a><span data-ttu-id="2e1ab-103">範囲を更新する</span><span class="sxs-lookup"><span data-stu-id="2e1ab-103">Update range</span></span>

<span data-ttu-id="2e1ab-104">範囲オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-104">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e1ab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2e1ab-105">Permissions</span></span>
<span data-ttu-id="2e1ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e1ab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e1ab-108">Permission type</span></span>      | <span data-ttu-id="2e1ab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e1ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e1ab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e1ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e1ab-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e1ab-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e1ab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e1ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e1ab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-113">Not supported.</span></span>    |
|<span data-ttu-id="2e1ab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e1ab-114">Application</span></span> | <span data-ttu-id="2e1ab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e1ab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e1ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="2e1ab-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e1ab-117">Optional request headers</span></span>
| <span data-ttu-id="2e1ab-118">名前</span><span class="sxs-lookup"><span data-stu-id="2e1ab-118">Name</span></span>       | <span data-ttu-id="2e1ab-119">説明</span><span class="sxs-lookup"><span data-stu-id="2e1ab-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2e1ab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e1ab-120">Authorization</span></span>  | <span data-ttu-id="2e1ab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e1ab-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2e1ab-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e1ab-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e1ab-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e1ab-126">Request body</span></span>
<span data-ttu-id="2e1ab-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e1ab-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e1ab-130">Property</span></span>     | <span data-ttu-id="2e1ab-131">型</span><span class="sxs-lookup"><span data-stu-id="2e1ab-131">Type</span></span>   |<span data-ttu-id="2e1ab-132">説明</span><span class="sxs-lookup"><span data-stu-id="2e1ab-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e1ab-133">columnHidden</span><span class="sxs-lookup"><span data-stu-id="2e1ab-133">columnHidden</span></span>|<span data-ttu-id="2e1ab-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="2e1ab-134">boolean</span></span>|<span data-ttu-id="2e1ab-135">現在の範囲のすべての列が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-135">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="2e1ab-136">formulas</span><span class="sxs-lookup"><span data-stu-id="2e1ab-136">formulas</span></span>|<span data-ttu-id="2e1ab-137">Json</span><span class="sxs-lookup"><span data-stu-id="2e1ab-137">Json</span></span>|<span data-ttu-id="2e1ab-138">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-138">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="2e1ab-139">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="2e1ab-139">formulasLocal</span></span>|<span data-ttu-id="2e1ab-140">Json</span><span class="sxs-lookup"><span data-stu-id="2e1ab-140">Json</span></span>|<span data-ttu-id="2e1ab-p105">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="2e1ab-143">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="2e1ab-143">formulasR1C1</span></span>|<span data-ttu-id="2e1ab-144">Json</span><span class="sxs-lookup"><span data-stu-id="2e1ab-144">Json</span></span>|<span data-ttu-id="2e1ab-145">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-145">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="2e1ab-146">numberFormat</span><span class="sxs-lookup"><span data-stu-id="2e1ab-146">numberFormat</span></span>|<span data-ttu-id="2e1ab-147">Json</span><span class="sxs-lookup"><span data-stu-id="2e1ab-147">Json</span></span>|<span data-ttu-id="2e1ab-148">指定したセルの Excel の数値書式コードを表します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-148">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="2e1ab-149">rowHidden</span><span class="sxs-lookup"><span data-stu-id="2e1ab-149">rowHidden</span></span>|<span data-ttu-id="2e1ab-150">boolean</span><span class="sxs-lookup"><span data-stu-id="2e1ab-150">boolean</span></span>|<span data-ttu-id="2e1ab-151">現在の範囲のすべての行が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-151">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="2e1ab-152">values</span><span class="sxs-lookup"><span data-stu-id="2e1ab-152">values</span></span>|<span data-ttu-id="2e1ab-153">Json</span><span class="sxs-lookup"><span data-stu-id="2e1ab-153">Json</span></span>|<span data-ttu-id="2e1ab-p106">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="2e1ab-157">応答</span><span class="sxs-lookup"><span data-stu-id="2e1ab-157">Response</span></span>

<span data-ttu-id="2e1ab-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-158">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e1ab-159">例</span><span class="sxs-lookup"><span data-stu-id="2e1ab-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e1ab-160">要求</span><span class="sxs-lookup"><span data-stu-id="2e1ab-160">Request</span></span>
<span data-ttu-id="2e1ab-p107">以下は、要求の例です。値、数値書式、および数式の範囲が更新されます。`null` 入力は、その特定の入力用のセルを無視するように API に指示します。値、数値書式、および数式は、個別に更新したり、同じ API 呼び出しで一緒に結合したりできます。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="2e1ab-165">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2e1ab-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e1ab-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="2e1ab-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e1ab-167">応答</span><span class="sxs-lookup"><span data-stu-id="2e1ab-167">Response</span></span>
<span data-ttu-id="2e1ab-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2e1ab-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/range-update.md/update_range/numberFormat:
      Inconsistent types between parameter (Collection) and table (None)",
    "Warning: /api-reference/v1.0/api/range-update.md/update_range/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/range-update.md/update_range/numberFormat:
      Type mismatch between example and table. Parameter name: numberFormat; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Error: /api-reference/v1.0/api/range-update.md/update_range/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
