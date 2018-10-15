# <a name="chartcollection-add"></a><span data-ttu-id="b45b6-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="b45b6-101">ChartCollection: add</span></span>

<span data-ttu-id="b45b6-102">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="b45b6-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="b45b6-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b45b6-103">Permissions</span></span>
<span data-ttu-id="b45b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b45b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b45b6-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b45b6-106">Permission type</span></span>      | <span data-ttu-id="b45b6-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b45b6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b45b6-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b45b6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b45b6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b45b6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b45b6-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b45b6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b45b6-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b45b6-111">Not supported.</span></span>    |
|<span data-ttu-id="b45b6-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b45b6-112">Application</span></span> | <span data-ttu-id="b45b6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b45b6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b45b6-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b45b6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="b45b6-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b45b6-115">Request headers</span></span>
| <span data-ttu-id="b45b6-116">名前</span><span class="sxs-lookup"><span data-stu-id="b45b6-116">Name</span></span>       | <span data-ttu-id="b45b6-117">説明</span><span class="sxs-lookup"><span data-stu-id="b45b6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b45b6-118">承認</span><span class="sxs-lookup"><span data-stu-id="b45b6-118">Authorization</span></span>  | <span data-ttu-id="b45b6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b45b6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b45b6-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b45b6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b45b6-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b45b6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45b6-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b45b6-124">Request body</span></span>
<span data-ttu-id="b45b6-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b45b6-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b45b6-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b45b6-126">Parameter</span></span>    | <span data-ttu-id="b45b6-127">型</span><span class="sxs-lookup"><span data-stu-id="b45b6-127">Type</span></span>   |<span data-ttu-id="b45b6-128">説明</span><span class="sxs-lookup"><span data-stu-id="b45b6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b45b6-129">型</span><span class="sxs-lookup"><span data-stu-id="b45b6-129">type</span></span>|<span data-ttu-id="b45b6-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b45b6-130">string</span></span>|<span data-ttu-id="b45b6-131">グラフの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b45b6-131">Represents the name of a chart object.</span></span>  <span data-ttu-id="b45b6-132">指定できる値は、 `ColumnClustered`、 `ColumnStacked`、 `ColumnStacked100`、 `BarClustered`、 `BarStacked`、 `BarStacked100`、 `LineStacked`、 `LineStacked100`、 `LineMarkers`、 `LineMarkersStacked`、 `LineMarkersStacked100`、 `PieOfPie`、 `etc.` です。</span><span class="sxs-lookup"><span data-stu-id="b45b6-132">The possible values are `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, or `PieOfPie`.</span></span>|
|<span data-ttu-id="b45b6-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="b45b6-133">sourceData</span></span>|<span data-ttu-id="b45b6-134">Json</span><span class="sxs-lookup"><span data-stu-id="b45b6-134">Json</span></span>|<span data-ttu-id="b45b6-135">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b45b6-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="b45b6-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="b45b6-136">seriesBy</span></span>|<span data-ttu-id="b45b6-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b45b6-137">string</span></span>|<span data-ttu-id="b45b6-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b45b6-138">Optional.</span></span> <span data-ttu-id="b45b6-139">方法の列または行がグラフのデータ系列として使用されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b45b6-139">Returns or sets the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="b45b6-140">指定できる値は、 `Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="b45b6-140">The possible values are `Auto`, `Columns`, or `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="b45b6-141">応答</span><span class="sxs-lookup"><span data-stu-id="b45b6-141">Response</span></span>

<span data-ttu-id="b45b6-142">成功した場合、このメソッドは `200 OK`応答コードと、応答本文で [WorkbookChart](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b45b6-142">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b45b6-143">例</span><span class="sxs-lookup"><span data-stu-id="b45b6-143">Example</span></span>
<span data-ttu-id="b45b6-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b45b6-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b45b6-145">要求</span><span class="sxs-lookup"><span data-stu-id="b45b6-145">Request</span></span>
<span data-ttu-id="b45b6-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b45b6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="b45b6-147">応答</span><span class="sxs-lookup"><span data-stu-id="b45b6-147">Response</span></span>
<span data-ttu-id="b45b6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b45b6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
