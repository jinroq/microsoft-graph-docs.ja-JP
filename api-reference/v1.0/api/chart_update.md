# <a name="update-chart"></a><span data-ttu-id="f163d-101">Update chart</span><span class="sxs-lookup"><span data-stu-id="f163d-101">Update chart</span></span>

<span data-ttu-id="f163d-102">グラフ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f163d-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f163d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f163d-103">Permissions</span></span>
<span data-ttu-id="f163d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f163d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f163d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f163d-106">Permission type</span></span>      | <span data-ttu-id="f163d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f163d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f163d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f163d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f163d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f163d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f163d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f163d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f163d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f163d-111">Not supported.</span></span>    |
|<span data-ttu-id="f163d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f163d-112">Application</span></span> | <span data-ttu-id="f163d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f163d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f163d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f163d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="f163d-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f163d-115">Optional request headers</span></span>
| <span data-ttu-id="f163d-116">名前</span><span class="sxs-lookup"><span data-stu-id="f163d-116">Name</span></span>       | <span data-ttu-id="f163d-117">説明</span><span class="sxs-lookup"><span data-stu-id="f163d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f163d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="f163d-118">Authorization</span></span>  | <span data-ttu-id="f163d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f163d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f163d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f163d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="f163d-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f163d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f163d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f163d-124">Request body</span></span>
<span data-ttu-id="f163d-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f163d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f163d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f163d-128">Property</span></span>     | <span data-ttu-id="f163d-129">型</span><span class="sxs-lookup"><span data-stu-id="f163d-129">Type</span></span>   |<span data-ttu-id="f163d-130">説明</span><span class="sxs-lookup"><span data-stu-id="f163d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f163d-131">height</span><span class="sxs-lookup"><span data-stu-id="f163d-131">height</span></span>|<span data-ttu-id="f163d-132">double</span><span class="sxs-lookup"><span data-stu-id="f163d-132">double</span></span>|<span data-ttu-id="f163d-133">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="f163d-133">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="f163d-134">left</span><span class="sxs-lookup"><span data-stu-id="f163d-134">left</span></span>|<span data-ttu-id="f163d-135">double</span><span class="sxs-lookup"><span data-stu-id="f163d-135">double</span></span>|<span data-ttu-id="f163d-136">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="f163d-136">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="f163d-137">name</span><span class="sxs-lookup"><span data-stu-id="f163d-137">name</span></span>|<span data-ttu-id="f163d-138">string</span><span class="sxs-lookup"><span data-stu-id="f163d-138">string</span></span>|<span data-ttu-id="f163d-139"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="f163d-139">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="f163d-140">top</span><span class="sxs-lookup"><span data-stu-id="f163d-140">top</span></span>|<span data-ttu-id="f163d-141">double</span><span class="sxs-lookup"><span data-stu-id="f163d-141">double</span></span>|<span data-ttu-id="f163d-142">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="f163d-142">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="f163d-143">width</span><span class="sxs-lookup"><span data-stu-id="f163d-143">width</span></span>|<span data-ttu-id="f163d-144">double</span><span class="sxs-lookup"><span data-stu-id="f163d-144">double</span></span>|<span data-ttu-id="f163d-145">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="f163d-145">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="f163d-146">応答</span><span class="sxs-lookup"><span data-stu-id="f163d-146">Response</span></span>

<span data-ttu-id="f163d-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f163d-147">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f163d-148">例</span><span class="sxs-lookup"><span data-stu-id="f163d-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f163d-149">要求</span><span class="sxs-lookup"><span data-stu-id="f163d-149">Request</span></span>
<span data-ttu-id="f163d-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f163d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="f163d-151">応答</span><span class="sxs-lookup"><span data-stu-id="f163d-151">Response</span></span>
<span data-ttu-id="f163d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f163d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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