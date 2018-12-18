---
title: Update chartdatalabels
description: chartdatalabels オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: ce120b5f00867b337191a8ba0c55e71b93f56a12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362504"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="7d85f-103">Update chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="7d85f-103">Update chartdatalabels</span></span>

> <span data-ttu-id="7d85f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d85f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d85f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d85f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d85f-106">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d85f-106">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d85f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d85f-107">Permissions</span></span>
<span data-ttu-id="7d85f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d85f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d85f-110">Permission type</span></span>      | <span data-ttu-id="7d85f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d85f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d85f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d85f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d85f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d85f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d85f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d85f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d85f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d85f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d85f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d85f-116">Application</span></span> | <span data-ttu-id="7d85f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d85f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d85f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d85f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="7d85f-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d85f-119">Optional request headers</span></span>
| <span data-ttu-id="7d85f-120">名前</span><span class="sxs-lookup"><span data-stu-id="7d85f-120">Name</span></span>       | <span data-ttu-id="7d85f-121">説明</span><span class="sxs-lookup"><span data-stu-id="7d85f-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7d85f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d85f-122">Authorization</span></span>  | <span data-ttu-id="7d85f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d85f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d85f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d85f-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d85f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d85f-128">Request body</span></span>
<span data-ttu-id="7d85f-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7d85f-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d85f-132">Property</span></span>     | <span data-ttu-id="7d85f-133">種類</span><span class="sxs-lookup"><span data-stu-id="7d85f-133">Type</span></span>   |<span data-ttu-id="7d85f-134">説明</span><span class="sxs-lookup"><span data-stu-id="7d85f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d85f-135">position</span><span class="sxs-lookup"><span data-stu-id="7d85f-135">position</span></span>|<span data-ttu-id="7d85f-136">文字列</span><span class="sxs-lookup"><span data-stu-id="7d85f-136">string</span></span>|<span data-ttu-id="7d85f-p106">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p106">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="7d85f-139">separator</span><span class="sxs-lookup"><span data-stu-id="7d85f-139">separator</span></span>|<span data-ttu-id="7d85f-140">文字列</span><span class="sxs-lookup"><span data-stu-id="7d85f-140">string</span></span>|<span data-ttu-id="7d85f-141">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="7d85f-141">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="7d85f-142">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="7d85f-142">showBubbleSize</span></span>|<span data-ttu-id="7d85f-143">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-143">boolean</span></span>|<span data-ttu-id="7d85f-144">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-144">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="7d85f-145">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="7d85f-145">showCategoryName</span></span>|<span data-ttu-id="7d85f-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-146">boolean</span></span>|<span data-ttu-id="7d85f-147">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-147">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="7d85f-148">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="7d85f-148">showLegendKey</span></span>|<span data-ttu-id="7d85f-149">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-149">boolean</span></span>|<span data-ttu-id="7d85f-150">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-150">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="7d85f-151">showPercentage</span><span class="sxs-lookup"><span data-stu-id="7d85f-151">showPercentage</span></span>|<span data-ttu-id="7d85f-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-152">boolean</span></span>|<span data-ttu-id="7d85f-153">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-153">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="7d85f-154">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="7d85f-154">showSeriesName</span></span>|<span data-ttu-id="7d85f-155">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-155">boolean</span></span>|<span data-ttu-id="7d85f-156">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-156">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="7d85f-157">showValue</span><span class="sxs-lookup"><span data-stu-id="7d85f-157">showValue</span></span>|<span data-ttu-id="7d85f-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="7d85f-158">boolean</span></span>|<span data-ttu-id="7d85f-159">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7d85f-159">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="7d85f-160">応答</span><span class="sxs-lookup"><span data-stu-id="7d85f-160">Response</span></span>

<span data-ttu-id="7d85f-161">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartDataLabels](../resources/chartdatalabels.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d85f-161">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d85f-162">例</span><span class="sxs-lookup"><span data-stu-id="7d85f-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d85f-163">要求</span><span class="sxs-lookup"><span data-stu-id="7d85f-163">Request</span></span>
<span data-ttu-id="7d85f-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d85f-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7d85f-165">応答</span><span class="sxs-lookup"><span data-stu-id="7d85f-165">Response</span></span>
<span data-ttu-id="7d85f-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d85f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->