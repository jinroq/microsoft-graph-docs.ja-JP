---
title: Update chartdatalabels
description: chartdatalabels オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 84c2bda2bf07198bb51ea69d1cefdc3689df0261
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003589"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="42a59-103">Update chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="42a59-103">Update chartdatalabels</span></span>

<span data-ttu-id="42a59-104">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="42a59-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="42a59-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="42a59-105">Permissions</span></span>
<span data-ttu-id="42a59-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a59-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42a59-108">Permission type</span></span>      | <span data-ttu-id="42a59-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="42a59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42a59-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42a59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42a59-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42a59-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42a59-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42a59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42a59-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42a59-113">Not supported.</span></span>    |
|<span data-ttu-id="42a59-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42a59-114">Application</span></span> | <span data-ttu-id="42a59-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42a59-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42a59-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42a59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="42a59-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42a59-117">Optional request headers</span></span>
| <span data-ttu-id="42a59-118">名前</span><span class="sxs-lookup"><span data-stu-id="42a59-118">Name</span></span>       | <span data-ttu-id="42a59-119">説明</span><span class="sxs-lookup"><span data-stu-id="42a59-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="42a59-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="42a59-120">Authorization</span></span>  | <span data-ttu-id="42a59-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="42a59-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42a59-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42a59-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="42a59-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="42a59-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a59-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="42a59-126">Request body</span></span>
<span data-ttu-id="42a59-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="42a59-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="42a59-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42a59-130">Property</span></span>     | <span data-ttu-id="42a59-131">型</span><span class="sxs-lookup"><span data-stu-id="42a59-131">Type</span></span>   |<span data-ttu-id="42a59-132">説明</span><span class="sxs-lookup"><span data-stu-id="42a59-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42a59-133">position</span><span class="sxs-lookup"><span data-stu-id="42a59-133">position</span></span>|<span data-ttu-id="42a59-134">string</span><span class="sxs-lookup"><span data-stu-id="42a59-134">string</span></span>|<span data-ttu-id="42a59-135">データ ラベルの位置を表す DataLabelPosition 値。</span><span class="sxs-lookup"><span data-stu-id="42a59-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="42a59-136">使用可能な値は`None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、、 `Callout` `BestFit`です。</span><span class="sxs-lookup"><span data-stu-id="42a59-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="42a59-137">separator</span><span class="sxs-lookup"><span data-stu-id="42a59-137">separator</span></span>|<span data-ttu-id="42a59-138">string</span><span class="sxs-lookup"><span data-stu-id="42a59-138">string</span></span>|<span data-ttu-id="42a59-139">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="42a59-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="42a59-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="42a59-140">showBubbleSize</span></span>|<span data-ttu-id="42a59-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-141">boolean</span></span>|<span data-ttu-id="42a59-142">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="42a59-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="42a59-143">showCategoryName</span></span>|<span data-ttu-id="42a59-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-144">boolean</span></span>|<span data-ttu-id="42a59-145">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="42a59-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="42a59-146">showLegendKey</span></span>|<span data-ttu-id="42a59-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-147">boolean</span></span>|<span data-ttu-id="42a59-148">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="42a59-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="42a59-149">showPercentage</span></span>|<span data-ttu-id="42a59-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-150">boolean</span></span>|<span data-ttu-id="42a59-151">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="42a59-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="42a59-152">showSeriesName</span></span>|<span data-ttu-id="42a59-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-153">boolean</span></span>|<span data-ttu-id="42a59-154">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="42a59-155">showValue</span><span class="sxs-lookup"><span data-stu-id="42a59-155">showValue</span></span>|<span data-ttu-id="42a59-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="42a59-156">boolean</span></span>|<span data-ttu-id="42a59-157">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="42a59-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="42a59-158">応答</span><span class="sxs-lookup"><span data-stu-id="42a59-158">Response</span></span>

<span data-ttu-id="42a59-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookChartDataLabels](../resources/chartdatalabels.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42a59-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42a59-160">例</span><span class="sxs-lookup"><span data-stu-id="42a59-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42a59-161">要求</span><span class="sxs-lookup"><span data-stu-id="42a59-161">Request</span></span>
<span data-ttu-id="42a59-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42a59-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="42a59-163">プロトコル</span><span class="sxs-lookup"><span data-stu-id="42a59-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42a59-164">C#</span><span class="sxs-lookup"><span data-stu-id="42a59-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42a59-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="42a59-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42a59-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="42a59-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="42a59-167">Java</span><span class="sxs-lookup"><span data-stu-id="42a59-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="42a59-168">応答</span><span class="sxs-lookup"><span data-stu-id="42a59-168">Response</span></span>
<span data-ttu-id="42a59-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42a59-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
