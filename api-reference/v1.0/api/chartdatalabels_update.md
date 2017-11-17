# <a name="update-chartdatalabels"></a><span data-ttu-id="fe1c2-101">Update chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="fe1c2-101">Update chartdatalabels</span></span>

<span data-ttu-id="fe1c2-102">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe1c2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe1c2-103">Permissions</span></span>
<span data-ttu-id="fe1c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe1c2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe1c2-106">Permission type</span></span>      | <span data-ttu-id="fe1c2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe1c2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe1c2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe1c2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fe1c2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe1c2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe1c2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe1c2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe1c2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-111">Not supported.</span></span>    |
|<span data-ttu-id="fe1c2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe1c2-112">Application</span></span> | <span data-ttu-id="fe1c2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe1c2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe1c2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="fe1c2-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe1c2-115">Optional request headers</span></span>
| <span data-ttu-id="fe1c2-116">名前</span><span class="sxs-lookup"><span data-stu-id="fe1c2-116">Name</span></span>       | <span data-ttu-id="fe1c2-117">説明</span><span class="sxs-lookup"><span data-stu-id="fe1c2-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fe1c2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe1c2-118">Authorization</span></span>  | <span data-ttu-id="fe1c2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe1c2-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe1c2-121">Request body</span></span>
<span data-ttu-id="fe1c2-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fe1c2-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe1c2-125">Property</span></span>     | <span data-ttu-id="fe1c2-126">型</span><span class="sxs-lookup"><span data-stu-id="fe1c2-126">Type</span></span>   |<span data-ttu-id="fe1c2-127">説明</span><span class="sxs-lookup"><span data-stu-id="fe1c2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe1c2-128">position</span><span class="sxs-lookup"><span data-stu-id="fe1c2-128">position</span></span>|<span data-ttu-id="fe1c2-129">string</span><span class="sxs-lookup"><span data-stu-id="fe1c2-129">string</span></span>|<span data-ttu-id="fe1c2-p104">データ ラベルの位置を表す DataLabelPosition 値。可能な値は、`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout` です。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-p104">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="fe1c2-132">separator</span><span class="sxs-lookup"><span data-stu-id="fe1c2-132">separator</span></span>|<span data-ttu-id="fe1c2-133">string</span><span class="sxs-lookup"><span data-stu-id="fe1c2-133">string</span></span>|<span data-ttu-id="fe1c2-134">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-134">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="fe1c2-135">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="fe1c2-135">showBubbleSize</span></span>|<span data-ttu-id="fe1c2-136">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-136">boolean</span></span>|<span data-ttu-id="fe1c2-137">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-137">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="fe1c2-138">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="fe1c2-138">showCategoryName</span></span>|<span data-ttu-id="fe1c2-139">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-139">boolean</span></span>|<span data-ttu-id="fe1c2-140">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-140">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="fe1c2-141">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="fe1c2-141">showLegendKey</span></span>|<span data-ttu-id="fe1c2-142">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-142">boolean</span></span>|<span data-ttu-id="fe1c2-143">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-143">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="fe1c2-144">showPercentage</span><span class="sxs-lookup"><span data-stu-id="fe1c2-144">showPercentage</span></span>|<span data-ttu-id="fe1c2-145">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-145">boolean</span></span>|<span data-ttu-id="fe1c2-146">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-146">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="fe1c2-147">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="fe1c2-147">showSeriesName</span></span>|<span data-ttu-id="fe1c2-148">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-148">boolean</span></span>|<span data-ttu-id="fe1c2-149">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-149">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="fe1c2-150">showValue</span><span class="sxs-lookup"><span data-stu-id="fe1c2-150">showValue</span></span>|<span data-ttu-id="fe1c2-151">boolean</span><span class="sxs-lookup"><span data-stu-id="fe1c2-151">boolean</span></span>|<span data-ttu-id="fe1c2-152">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-152">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="fe1c2-153">応答</span><span class="sxs-lookup"><span data-stu-id="fe1c2-153">Response</span></span>

<span data-ttu-id="fe1c2-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartDataLabels](../resources/chartdatalabels.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-154">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe1c2-155">例</span><span class="sxs-lookup"><span data-stu-id="fe1c2-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe1c2-156">要求</span><span class="sxs-lookup"><span data-stu-id="fe1c2-156">Request</span></span>
<span data-ttu-id="fe1c2-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="fe1c2-158">応答</span><span class="sxs-lookup"><span data-stu-id="fe1c2-158">Response</span></span>
<span data-ttu-id="fe1c2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe1c2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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