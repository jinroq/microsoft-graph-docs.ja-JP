---
title: 範囲を更新する
description: 範囲オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2e92138aca64df0b39ee5afc04adeba2ab9f9eae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846005"
---
# <a name="update-range"></a><span data-ttu-id="cb385-103">範囲を更新する</span><span class="sxs-lookup"><span data-stu-id="cb385-103">Update range</span></span>

> <span data-ttu-id="cb385-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb385-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb385-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb385-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb385-106">範囲オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb385-106">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb385-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cb385-107">Permissions</span></span>
<span data-ttu-id="cb385-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb385-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cb385-110">Permission type</span></span>      | <span data-ttu-id="cb385-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cb385-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb385-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cb385-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb385-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb385-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cb385-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cb385-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb385-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb385-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cb385-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cb385-116">Application</span></span> | <span data-ttu-id="cb385-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb385-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb385-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cb385-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="cb385-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cb385-119">Optional request headers</span></span>
| <span data-ttu-id="cb385-120">名前</span><span class="sxs-lookup"><span data-stu-id="cb385-120">Name</span></span>       | <span data-ttu-id="cb385-121">説明</span><span class="sxs-lookup"><span data-stu-id="cb385-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cb385-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb385-122">Authorization</span></span>  | <span data-ttu-id="cb385-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cb385-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb385-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cb385-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cb385-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cb385-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb385-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="cb385-128">Request body</span></span>
<span data-ttu-id="cb385-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cb385-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cb385-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb385-132">Property</span></span>     | <span data-ttu-id="cb385-133">種類</span><span class="sxs-lookup"><span data-stu-id="cb385-133">Type</span></span>   |<span data-ttu-id="cb385-134">説明</span><span class="sxs-lookup"><span data-stu-id="cb385-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb385-135">columnHidden</span><span class="sxs-lookup"><span data-stu-id="cb385-135">columnHidden</span></span>|<span data-ttu-id="cb385-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb385-136">boolean</span></span>|<span data-ttu-id="cb385-137">現在の範囲のすべての列が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="cb385-137">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="cb385-138">formulas</span><span class="sxs-lookup"><span data-stu-id="cb385-138">formulas</span></span>|<span data-ttu-id="cb385-139">json</span><span class="sxs-lookup"><span data-stu-id="cb385-139">json</span></span>|<span data-ttu-id="cb385-140">A1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="cb385-140">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="cb385-141">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="cb385-141">formulasLocal</span></span>|<span data-ttu-id="cb385-142">json</span><span class="sxs-lookup"><span data-stu-id="cb385-142">json</span></span>|<span data-ttu-id="cb385-p106">ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。</span><span class="sxs-lookup"><span data-stu-id="cb385-p106">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="cb385-145">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="cb385-145">formulasR1C1</span></span>|<span data-ttu-id="cb385-146">json</span><span class="sxs-lookup"><span data-stu-id="cb385-146">json</span></span>|<span data-ttu-id="cb385-147">R1C1 スタイル表記の数式を表します。</span><span class="sxs-lookup"><span data-stu-id="cb385-147">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="cb385-148">numberFormat</span><span class="sxs-lookup"><span data-stu-id="cb385-148">numberFormat</span></span>|<span data-ttu-id="cb385-149">json</span><span class="sxs-lookup"><span data-stu-id="cb385-149">json</span></span>|<span data-ttu-id="cb385-150">指定したセルの Excel の数値書式コードを表します。</span><span class="sxs-lookup"><span data-stu-id="cb385-150">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="cb385-151">rowHidden</span><span class="sxs-lookup"><span data-stu-id="cb385-151">rowHidden</span></span>|<span data-ttu-id="cb385-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="cb385-152">boolean</span></span>|<span data-ttu-id="cb385-153">現在の範囲のすべての行が非表示になっているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="cb385-153">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="cb385-154">values</span><span class="sxs-lookup"><span data-stu-id="cb385-154">values</span></span>|<span data-ttu-id="cb385-155">json</span><span class="sxs-lookup"><span data-stu-id="cb385-155">json</span></span>|<span data-ttu-id="cb385-p107">指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="cb385-p107">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="cb385-159">応答</span><span class="sxs-lookup"><span data-stu-id="cb385-159">Response</span></span>

<span data-ttu-id="cb385-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cb385-160">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb385-161">例</span><span class="sxs-lookup"><span data-stu-id="cb385-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb385-162">要求</span><span class="sxs-lookup"><span data-stu-id="cb385-162">Request</span></span>
<span data-ttu-id="cb385-p108">以下は、要求の例です。値、数値書式、および数式の範囲が更新されます。`null` 入力は、その特定の入力用のセルを無視するように API に指示します。値、数値書式、および数式は、個別に更新したり、同じ API 呼び出しで一緒に結合したりできます。</span><span class="sxs-lookup"><span data-stu-id="cb385-p108">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="cb385-167">応答</span><span class="sxs-lookup"><span data-stu-id="cb385-167">Response</span></span>
<span data-ttu-id="cb385-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cb385-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "tocPath": ""
}-->
