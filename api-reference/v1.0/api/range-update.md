---
title: 範囲を更新する
description: 範囲オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: 3af876a73a8e7c401512c9aafc38e677769f868e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354951"
---
# <a name="update-range"></a><span data-ttu-id="a8376-103">範囲を更新する</span><span class="sxs-lookup"><span data-stu-id="a8376-103">Update range</span></span>

<span data-ttu-id="a8376-104">範囲オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8376-104">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8376-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a8376-105">Permissions</span></span>
<span data-ttu-id="a8376-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8376-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8376-108">Permission type</span></span>      | <span data-ttu-id="a8376-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8376-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8376-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8376-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8376-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8376-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8376-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8376-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8376-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8376-113">Not supported.</span></span>    |
|<span data-ttu-id="a8376-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8376-114">Application</span></span> | <span data-ttu-id="a8376-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8376-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8376-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8376-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="a8376-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8376-117">Optional request headers</span></span>
| <span data-ttu-id="a8376-118">名前</span><span class="sxs-lookup"><span data-stu-id="a8376-118">Name</span></span>       | <span data-ttu-id="a8376-119">説明</span><span class="sxs-lookup"><span data-stu-id="a8376-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a8376-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8376-120">Authorization</span></span>  | <span data-ttu-id="a8376-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a8376-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8376-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a8376-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a8376-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a8376-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8376-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8376-126">Request body</span></span>
<span data-ttu-id="a8376-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a8376-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a8376-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8376-130">Property</span></span>     | <span data-ttu-id="a8376-131">種類</span><span class="sxs-lookup"><span data-stu-id="a8376-131">Type</span></span>   |<span data-ttu-id="a8376-132">説明</span><span class="sxs-lookup"><span data-stu-id="a8376-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8376-133">columnHidden</span><span class="sxs-lookup"><span data-stu-id="a8376-133">columnHidden</span></span>|<span data-ttu-id="a8376-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="a8376-134">boolean</span></span>|<span data-ttu-id="a8376-135">現在の範囲のすべての列が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="a8376-135">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="a8376-136">formulas</span><span class="sxs-lookup"><span data-stu-id="a8376-136">formulas</span></span>|<span data-ttu-id="a8376-137">Json</span><span class="sxs-lookup"><span data-stu-id="a8376-137">Json</span></span>|<span data-ttu-id="a8376-138">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="a8376-138">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="a8376-139">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="a8376-139">formulasLocal</span></span>|<span data-ttu-id="a8376-140">Json</span><span class="sxs-lookup"><span data-stu-id="a8376-140">Json</span></span>|<span data-ttu-id="a8376-p105">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="a8376-p105">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="a8376-143">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="a8376-143">formulasR1C1</span></span>|<span data-ttu-id="a8376-144">Json</span><span class="sxs-lookup"><span data-stu-id="a8376-144">Json</span></span>|<span data-ttu-id="a8376-145">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="a8376-145">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="a8376-146">numberFormat</span><span class="sxs-lookup"><span data-stu-id="a8376-146">numberFormat</span></span>|<span data-ttu-id="a8376-147">Json</span><span class="sxs-lookup"><span data-stu-id="a8376-147">Json</span></span>|<span data-ttu-id="a8376-148">指定したセルの Excel の数値書式コードを表します。</span><span class="sxs-lookup"><span data-stu-id="a8376-148">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="a8376-149">rowHidden</span><span class="sxs-lookup"><span data-stu-id="a8376-149">rowHidden</span></span>|<span data-ttu-id="a8376-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="a8376-150">boolean</span></span>|<span data-ttu-id="a8376-151">現在の範囲のすべての行が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="a8376-151">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="a8376-152">values</span><span class="sxs-lookup"><span data-stu-id="a8376-152">values</span></span>|<span data-ttu-id="a8376-153">Json</span><span class="sxs-lookup"><span data-stu-id="a8376-153">Json</span></span>|<span data-ttu-id="a8376-p106">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="a8376-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="a8376-157">応答</span><span class="sxs-lookup"><span data-stu-id="a8376-157">Response</span></span>

<span data-ttu-id="a8376-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8376-158">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8376-159">例</span><span class="sxs-lookup"><span data-stu-id="a8376-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8376-160">要求</span><span class="sxs-lookup"><span data-stu-id="a8376-160">Request</span></span>
<span data-ttu-id="a8376-p107">以下は、要求の例です。値、数値書式、および数式の範囲が更新されます。`null` 入力は、その特定の入力用のセルを無視するように API に指示します。値、数値書式、および数式は、個別に更新したり、同じ API 呼び出しで一緒に結合したりできます。</span><span class="sxs-lookup"><span data-stu-id="a8376-p107">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="a8376-165">応答</span><span class="sxs-lookup"><span data-stu-id="a8376-165">Response</span></span>
<span data-ttu-id="a8376-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8376-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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