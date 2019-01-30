---
title: Update chartdatalabels
description: chartdatalabels オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b7eb067bed747ae2532939e61a9e0dec58ff4655
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640134"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="65f2b-103">Update chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="65f2b-103">Update chartdatalabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65f2b-104">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="65f2b-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="65f2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65f2b-105">Permissions</span></span>
<span data-ttu-id="65f2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65f2b-108">Permission type</span></span>      | <span data-ttu-id="65f2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65f2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65f2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65f2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65f2b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65f2b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65f2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65f2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65f2b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65f2b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="65f2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65f2b-114">Application</span></span> | <span data-ttu-id="65f2b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65f2b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65f2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65f2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="65f2b-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65f2b-117">Optional request headers</span></span>
| <span data-ttu-id="65f2b-118">名前</span><span class="sxs-lookup"><span data-stu-id="65f2b-118">Name</span></span>       | <span data-ttu-id="65f2b-119">説明</span><span class="sxs-lookup"><span data-stu-id="65f2b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="65f2b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65f2b-120">Authorization</span></span>  | <span data-ttu-id="65f2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65f2b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="65f2b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="65f2b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f2b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="65f2b-126">Request body</span></span>
<span data-ttu-id="65f2b-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="65f2b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65f2b-130">Property</span></span>     | <span data-ttu-id="65f2b-131">型</span><span class="sxs-lookup"><span data-stu-id="65f2b-131">Type</span></span>   |<span data-ttu-id="65f2b-132">説明</span><span class="sxs-lookup"><span data-stu-id="65f2b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65f2b-133">position</span><span class="sxs-lookup"><span data-stu-id="65f2b-133">position</span></span>|<span data-ttu-id="65f2b-134">文字列</span><span class="sxs-lookup"><span data-stu-id="65f2b-134">string</span></span>|<span data-ttu-id="65f2b-p105">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="65f2b-137">separator</span><span class="sxs-lookup"><span data-stu-id="65f2b-137">separator</span></span>|<span data-ttu-id="65f2b-138">文字列</span><span class="sxs-lookup"><span data-stu-id="65f2b-138">string</span></span>|<span data-ttu-id="65f2b-139">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="65f2b-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="65f2b-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="65f2b-140">showBubbleSize</span></span>|<span data-ttu-id="65f2b-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-141">boolean</span></span>|<span data-ttu-id="65f2b-142">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="65f2b-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="65f2b-143">showCategoryName</span></span>|<span data-ttu-id="65f2b-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-144">boolean</span></span>|<span data-ttu-id="65f2b-145">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="65f2b-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="65f2b-146">showLegendKey</span></span>|<span data-ttu-id="65f2b-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-147">boolean</span></span>|<span data-ttu-id="65f2b-148">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="65f2b-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="65f2b-149">showPercentage</span></span>|<span data-ttu-id="65f2b-150">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-150">boolean</span></span>|<span data-ttu-id="65f2b-151">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="65f2b-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="65f2b-152">showSeriesName</span></span>|<span data-ttu-id="65f2b-153">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-153">boolean</span></span>|<span data-ttu-id="65f2b-154">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="65f2b-155">showValue</span><span class="sxs-lookup"><span data-stu-id="65f2b-155">showValue</span></span>|<span data-ttu-id="65f2b-156">ブール値</span><span class="sxs-lookup"><span data-stu-id="65f2b-156">boolean</span></span>|<span data-ttu-id="65f2b-157">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="65f2b-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="65f2b-158">応答</span><span class="sxs-lookup"><span data-stu-id="65f2b-158">Response</span></span>

<span data-ttu-id="65f2b-159">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartDataLabels](../resources/chartdatalabels.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="65f2b-159">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65f2b-160">例</span><span class="sxs-lookup"><span data-stu-id="65f2b-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65f2b-161">要求</span><span class="sxs-lookup"><span data-stu-id="65f2b-161">Request</span></span>
<span data-ttu-id="65f2b-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="65f2b-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="65f2b-163">応答</span><span class="sxs-lookup"><span data-stu-id="65f2b-163">Response</span></span>
<span data-ttu-id="65f2b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="65f2b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
