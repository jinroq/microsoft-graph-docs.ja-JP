# <a name="chart-image"></a><span data-ttu-id="8b8df-101">グラフ:画像</span><span class="sxs-lookup"><span data-stu-id="8b8df-101">Chart: Image</span></span>

<span data-ttu-id="8b8df-102">指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="8b8df-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b8df-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b8df-103">Permissions</span></span>
<span data-ttu-id="8b8df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b8df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b8df-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b8df-106">Permission type</span></span>      | <span data-ttu-id="8b8df-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b8df-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b8df-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b8df-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8b8df-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b8df-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b8df-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b8df-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8df-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b8df-111">Not supported.</span></span>    |
|<span data-ttu-id="8b8df-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b8df-112">Application</span></span> | <span data-ttu-id="8b8df-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b8df-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8df-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b8df-114">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="8b8df-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b8df-115">Request headers</span></span>
| <span data-ttu-id="8b8df-116">名前</span><span class="sxs-lookup"><span data-stu-id="8b8df-116">Name</span></span>       | <span data-ttu-id="8b8df-117">説明</span><span class="sxs-lookup"><span data-stu-id="8b8df-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b8df-118">承認</span><span class="sxs-lookup"><span data-stu-id="8b8df-118">Authorization</span></span>  | <span data-ttu-id="8b8df-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b8df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b8df-121">ワークブック-セッション-ID</span><span class="sxs-lookup"><span data-stu-id="8b8df-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b8df-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8b8df-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="8b8df-124">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b8df-124">Path parameters</span></span>
<span data-ttu-id="8b8df-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b8df-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b8df-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b8df-126">Parameter</span></span>    | <span data-ttu-id="8b8df-127">型</span><span class="sxs-lookup"><span data-stu-id="8b8df-127">Type</span></span>   |<span data-ttu-id="8b8df-128">説明</span><span class="sxs-lookup"><span data-stu-id="8b8df-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b8df-129">高さ</span><span class="sxs-lookup"><span data-stu-id="8b8df-129">height</span></span>|<span data-ttu-id="8b8df-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8b8df-130">Int32</span></span>|<span data-ttu-id="8b8df-131">結果の画像が希望する高さ。</span><span class="sxs-lookup"><span data-stu-id="8b8df-131">Optional. The desired height of the resulting image.</span></span> <span data-ttu-id="8b8df-132">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8b8df-132">Optional.</span></span>|
|<span data-ttu-id="8b8df-133">幅</span><span class="sxs-lookup"><span data-stu-id="8b8df-133">width</span></span>|<span data-ttu-id="8b8df-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8b8df-134">Int32</span></span>|<span data-ttu-id="8b8df-135">結果の画像が希望する幅。</span><span class="sxs-lookup"><span data-stu-id="8b8df-135">Optional. The desired width of the resulting image.</span></span> <span data-ttu-id="8b8df-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8b8df-136">Optional.</span></span>|
|<span data-ttu-id="8b8df-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="8b8df-137">fittingMode</span></span>|<span data-ttu-id="8b8df-138">文字列</span><span class="sxs-lookup"><span data-stu-id="8b8df-138">string</span></span>|<span data-ttu-id="8b8df-139">メソッド (高さと幅の両方が設定されている) 場合は、グラフを指定のサイズを拡大または縮小するために使用します。」</span><span class="sxs-lookup"><span data-stu-id="8b8df-139">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: , , .</span></span>  <span data-ttu-id="8b8df-140">可能な値は、`Fit`、`FitAndCenter`、`Fill` です。</span><span class="sxs-lookup"><span data-stu-id="8b8df-140">The possible values are `Fit`, `FitAndCenter`, or `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="8b8df-141">応答</span><span class="sxs-lookup"><span data-stu-id="8b8df-141">Response</span></span>

<span data-ttu-id="8b8df-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。</span><span class="sxs-lookup"><span data-stu-id="8b8df-142">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b8df-143">例</span><span class="sxs-lookup"><span data-stu-id="8b8df-143">Example</span></span>
<span data-ttu-id="8b8df-144">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8b8df-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8b8df-145">要求</span><span class="sxs-lookup"><span data-stu-id="8b8df-145">Request</span></span>
<span data-ttu-id="8b8df-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b8df-146">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="8b8df-147">応答</span><span class="sxs-lookup"><span data-stu-id="8b8df-147">Response</span></span>
<span data-ttu-id="8b8df-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8b8df-148">Here is an example of the response.</span></span> <span data-ttu-id="8b8df-149">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b8df-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8b8df-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8b8df-150">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="8b8df-151">使用例</span><span class="sxs-lookup"><span data-stu-id="8b8df-151">Usage</span></span>

<span data-ttu-id="8b8df-152">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="8b8df-152">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="8b8df-153">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="8b8df-153">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="8b8df-154">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8b8df-154">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="8b8df-156">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b8df-156">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="8b8df-157">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="8b8df-157">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
