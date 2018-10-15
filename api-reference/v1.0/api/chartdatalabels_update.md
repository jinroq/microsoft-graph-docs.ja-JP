# <a name="update-chartdatalabels"></a><span data-ttu-id="cec83-101">chartdatalabels を更新する</span><span class="sxs-lookup"><span data-stu-id="cec83-101">Update chartdatalabels</span></span>

<span data-ttu-id="cec83-102">chartdatalabels オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cec83-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cec83-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cec83-103">Permissions</span></span>
<span data-ttu-id="cec83-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cec83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cec83-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cec83-106">Permission type</span></span>      | <span data-ttu-id="cec83-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cec83-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cec83-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cec83-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cec83-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cec83-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cec83-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cec83-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cec83-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cec83-111">Not supported.</span></span>    |
|<span data-ttu-id="cec83-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cec83-112">Application</span></span> | <span data-ttu-id="cec83-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cec83-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cec83-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cec83-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="cec83-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cec83-115">Optional request headers</span></span>
| <span data-ttu-id="cec83-116">名前</span><span class="sxs-lookup"><span data-stu-id="cec83-116">Name</span></span>       | <span data-ttu-id="cec83-117">説明</span><span class="sxs-lookup"><span data-stu-id="cec83-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cec83-118">承認</span><span class="sxs-lookup"><span data-stu-id="cec83-118">Authorization</span></span>  | <span data-ttu-id="cec83-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cec83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cec83-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cec83-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="cec83-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cec83-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec83-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="cec83-124">Request body</span></span>
<span data-ttu-id="cec83-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cec83-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cec83-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cec83-128">Property</span></span>     | <span data-ttu-id="cec83-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="cec83-129">Type</span></span>   |<span data-ttu-id="cec83-130">説明</span><span class="sxs-lookup"><span data-stu-id="cec83-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cec83-131">position</span><span class="sxs-lookup"><span data-stu-id="cec83-131">position</span></span>|<span data-ttu-id="cec83-132">string</span><span class="sxs-lookup"><span data-stu-id="cec83-132">string</span></span>|<span data-ttu-id="cec83-133">データ ラベルの位置を表す DataLabelPosition 値。</span><span class="sxs-lookup"><span data-stu-id="cec83-133">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="cec83-134">可能な値は、`None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout` です。</span><span class="sxs-lookup"><span data-stu-id="cec83-134">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="cec83-135">separator</span><span class="sxs-lookup"><span data-stu-id="cec83-135">separator</span></span>|<span data-ttu-id="cec83-136">string</span><span class="sxs-lookup"><span data-stu-id="cec83-136">string</span></span>|<span data-ttu-id="cec83-137">グラフのデータ ラベルに使用される区切り文字を表す文字列を設定します。</span><span class="sxs-lookup"><span data-stu-id="cec83-137">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="cec83-138">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="cec83-138">showBubbleSize</span></span>|<span data-ttu-id="cec83-139">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-139">boolean</span></span>|<span data-ttu-id="cec83-140">データ ラベルのバブルのサイズを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-140">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="cec83-141">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="cec83-141">showCategoryName</span></span>|<span data-ttu-id="cec83-142">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-142">boolean</span></span>|<span data-ttu-id="cec83-143">データ ラベルのカテゴリ名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-143">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="cec83-144">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="cec83-144">showLegendKey</span></span>|<span data-ttu-id="cec83-145">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-145">boolean</span></span>|<span data-ttu-id="cec83-146">データ ラベルの凡例マーカーを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-146">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="cec83-147">showPercentage</span><span class="sxs-lookup"><span data-stu-id="cec83-147">showPercentage</span></span>|<span data-ttu-id="cec83-148">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-148">boolean</span></span>|<span data-ttu-id="cec83-149">データ ラベルのパーセンテージを表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-149">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="cec83-150">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="cec83-150">showSeriesName</span></span>|<span data-ttu-id="cec83-151">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-151">boolean</span></span>|<span data-ttu-id="cec83-152">データ ラベルの系列名を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-152">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="cec83-153">showValue</span><span class="sxs-lookup"><span data-stu-id="cec83-153">showValue</span></span>|<span data-ttu-id="cec83-154">boolean</span><span class="sxs-lookup"><span data-stu-id="cec83-154">boolean</span></span>|<span data-ttu-id="cec83-155">データ ラベルの値を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="cec83-155">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="cec83-156">応答</span><span class="sxs-lookup"><span data-stu-id="cec83-156">Response</span></span>

<span data-ttu-id="cec83-157">成功した場合、このメソッドは `200 OK` 応答コードを返し、応答本文で[WorkbookChartDataLabels](../resources/chartdatalabels.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cec83-157">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cec83-158">例</span><span class="sxs-lookup"><span data-stu-id="cec83-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cec83-159">要求</span><span class="sxs-lookup"><span data-stu-id="cec83-159">Request</span></span>
<span data-ttu-id="cec83-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cec83-160">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cec83-161">応答</span><span class="sxs-lookup"><span data-stu-id="cec83-161">Response</span></span>
<span data-ttu-id="cec83-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cec83-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->