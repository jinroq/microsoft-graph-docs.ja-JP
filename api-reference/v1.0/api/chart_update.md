# <a name="update-chart"></a><span data-ttu-id="a1634-101">グラフを更新する</span><span class="sxs-lookup"><span data-stu-id="a1634-101">Update chart</span></span>

<span data-ttu-id="a1634-102">グラフ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1634-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1634-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1634-103">Permissions</span></span>
<span data-ttu-id="a1634-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1634-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1634-106">Permission type</span></span>      | <span data-ttu-id="a1634-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1634-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1634-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1634-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a1634-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1634-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a1634-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1634-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1634-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1634-111">Not supported.</span></span>    |
|<span data-ttu-id="a1634-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1634-112">Application</span></span> | <span data-ttu-id="a1634-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1634-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1634-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1634-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a1634-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1634-115">Optional request headers</span></span>
| <span data-ttu-id="a1634-116">名前</span><span class="sxs-lookup"><span data-stu-id="a1634-116">Name</span></span>       | <span data-ttu-id="a1634-117">説明</span><span class="sxs-lookup"><span data-stu-id="a1634-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a1634-118">承認</span><span class="sxs-lookup"><span data-stu-id="a1634-118">Authorization</span></span>  | <span data-ttu-id="a1634-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a1634-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1634-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a1634-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a1634-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a1634-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1634-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1634-124">Request body</span></span>
<span data-ttu-id="a1634-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a1634-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a1634-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1634-128">Property</span></span>     | <span data-ttu-id="a1634-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="a1634-129">Type</span></span>   |<span data-ttu-id="a1634-130">説明</span><span class="sxs-lookup"><span data-stu-id="a1634-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1634-131">height</span><span class="sxs-lookup"><span data-stu-id="a1634-131">height</span></span>|<span data-ttu-id="a1634-132">double</span><span class="sxs-lookup"><span data-stu-id="a1634-132">double</span></span>|<span data-ttu-id="a1634-133">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a1634-133">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="a1634-134">left</span><span class="sxs-lookup"><span data-stu-id="a1634-134">left</span></span>|<span data-ttu-id="a1634-135">double</span><span class="sxs-lookup"><span data-stu-id="a1634-135">double</span></span>|<span data-ttu-id="a1634-136">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="a1634-136">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="a1634-137">name</span><span class="sxs-lookup"><span data-stu-id="a1634-137">name</span></span>|<span data-ttu-id="a1634-138">文字列</span><span class="sxs-lookup"><span data-stu-id="a1634-138">string</span></span>|<span data-ttu-id="a1634-139">グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a1634-139">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="a1634-140">top</span><span class="sxs-lookup"><span data-stu-id="a1634-140">top</span></span>|<span data-ttu-id="a1634-141">double</span><span class="sxs-lookup"><span data-stu-id="a1634-141">double</span></span>|<span data-ttu-id="a1634-142">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a1634-142">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="a1634-143">width</span><span class="sxs-lookup"><span data-stu-id="a1634-143">width</span></span>|<span data-ttu-id="a1634-144">double</span><span class="sxs-lookup"><span data-stu-id="a1634-144">double</span></span>|<span data-ttu-id="a1634-145">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="a1634-145">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="a1634-146">応答</span><span class="sxs-lookup"><span data-stu-id="a1634-146">Response</span></span>

<span data-ttu-id="a1634-147">成功した場合、このメソッドは `200 OK` 応答コードを返し、応答本文で [WorkbookChart](../resources/chart.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1634-147">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1634-148">例</span><span class="sxs-lookup"><span data-stu-id="a1634-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1634-149">要求</span><span class="sxs-lookup"><span data-stu-id="a1634-149">Request</span></span>
<span data-ttu-id="a1634-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1634-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="a1634-151">応答</span><span class="sxs-lookup"><span data-stu-id="a1634-151">Response</span></span>
<span data-ttu-id="a1634-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1634-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->