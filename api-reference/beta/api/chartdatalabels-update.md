---
title: WorkbookChartDataLabels の更新
description: Workbookchartdatalabels オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d4ba0d703f4dee429404ee02939b3917064ab8f7
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635569"
---
# <a name="update-workbookchartdatalabels"></a><span data-ttu-id="9aa10-103">WorkbookChartDataLabels の更新</span><span class="sxs-lookup"><span data-stu-id="9aa10-103">Update workbookChartDataLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa10-104">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9aa10-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9aa10-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9aa10-105">Permissions</span></span>
<span data-ttu-id="9aa10-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aa10-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9aa10-108">Permission type</span></span>      | <span data-ttu-id="9aa10-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9aa10-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9aa10-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9aa10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9aa10-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9aa10-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9aa10-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9aa10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9aa10-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9aa10-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9aa10-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9aa10-114">Application</span></span> | <span data-ttu-id="9aa10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9aa10-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9aa10-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9aa10-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="9aa10-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9aa10-117">Optional request headers</span></span>
| <span data-ttu-id="9aa10-118">名前</span><span class="sxs-lookup"><span data-stu-id="9aa10-118">Name</span></span>       | <span data-ttu-id="9aa10-119">説明</span><span class="sxs-lookup"><span data-stu-id="9aa10-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9aa10-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aa10-120">Authorization</span></span>  | <span data-ttu-id="9aa10-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9aa10-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9aa10-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9aa10-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aa10-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9aa10-126">Request body</span></span>
<span data-ttu-id="9aa10-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9aa10-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9aa10-130">Property</span></span>     | <span data-ttu-id="9aa10-131">型</span><span class="sxs-lookup"><span data-stu-id="9aa10-131">Type</span></span>   |<span data-ttu-id="9aa10-132">説明</span><span class="sxs-lookup"><span data-stu-id="9aa10-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aa10-133">position</span><span class="sxs-lookup"><span data-stu-id="9aa10-133">position</span></span>|<span data-ttu-id="9aa10-134">string</span><span class="sxs-lookup"><span data-stu-id="9aa10-134">string</span></span>|<span data-ttu-id="9aa10-p105">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="9aa10-137">separator</span><span class="sxs-lookup"><span data-stu-id="9aa10-137">separator</span></span>|<span data-ttu-id="9aa10-138">string</span><span class="sxs-lookup"><span data-stu-id="9aa10-138">string</span></span>|<span data-ttu-id="9aa10-139">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="9aa10-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="9aa10-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="9aa10-140">showBubbleSize</span></span>|<span data-ttu-id="9aa10-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-141">boolean</span></span>|<span data-ttu-id="9aa10-142">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="9aa10-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="9aa10-143">showCategoryName</span></span>|<span data-ttu-id="9aa10-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-144">boolean</span></span>|<span data-ttu-id="9aa10-145">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="9aa10-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="9aa10-146">showLegendKey</span></span>|<span data-ttu-id="9aa10-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-147">boolean</span></span>|<span data-ttu-id="9aa10-148">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="9aa10-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="9aa10-149">showPercentage</span></span>|<span data-ttu-id="9aa10-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-150">boolean</span></span>|<span data-ttu-id="9aa10-151">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="9aa10-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="9aa10-152">showSeriesName</span></span>|<span data-ttu-id="9aa10-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-153">boolean</span></span>|<span data-ttu-id="9aa10-154">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="9aa10-155">showValue</span><span class="sxs-lookup"><span data-stu-id="9aa10-155">showValue</span></span>|<span data-ttu-id="9aa10-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="9aa10-156">boolean</span></span>|<span data-ttu-id="9aa10-157">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9aa10-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="9aa10-158">応答</span><span class="sxs-lookup"><span data-stu-id="9aa10-158">Response</span></span>

<span data-ttu-id="9aa10-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookChartDataLabels](../resources/workbookchartdatalabels.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9aa10-159">If successful, this method returns a `200 OK` response code and updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9aa10-160">例</span><span class="sxs-lookup"><span data-stu-id="9aa10-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9aa10-161">要求</span><span class="sxs-lookup"><span data-stu-id="9aa10-161">Request</span></span>
<span data-ttu-id="9aa10-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9aa10-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
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
##### <a name="response"></a><span data-ttu-id="9aa10-163">応答</span><span class="sxs-lookup"><span data-stu-id="9aa10-163">Response</span></span>
<span data-ttu-id="9aa10-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9aa10-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9aa10-167">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="9aa10-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9aa10-168">Visual</span><span class="sxs-lookup"><span data-stu-id="9aa10-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9aa10-169">Java</span><span class="sxs-lookup"><span data-stu-id="9aa10-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
