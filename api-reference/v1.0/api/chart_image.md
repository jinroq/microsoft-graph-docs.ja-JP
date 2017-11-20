# <a name="chart-image"></a><span data-ttu-id="bfc66-101">グラフ:画像</span><span class="sxs-lookup"><span data-stu-id="bfc66-101">Chart: Image</span></span>

<span data-ttu-id="bfc66-102">指定したサイズに合わせてグラフを拡大、縮小することで、グラフを Base64 でエンコードされた画像としてレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="bfc66-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfc66-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bfc66-103">Permissions</span></span>
<span data-ttu-id="bfc66-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bfc66-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bfc66-106">Permission type</span></span>      | <span data-ttu-id="bfc66-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bfc66-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc66-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bfc66-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bfc66-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfc66-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfc66-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bfc66-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc66-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfc66-111">Not supported.</span></span>    |
|<span data-ttu-id="bfc66-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bfc66-112">Application</span></span> | <span data-ttu-id="bfc66-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfc66-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfc66-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bfc66-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="bfc66-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfc66-115">Request headers</span></span>
| <span data-ttu-id="bfc66-116">名前</span><span class="sxs-lookup"><span data-stu-id="bfc66-116">Name</span></span>       | <span data-ttu-id="bfc66-117">説明</span><span class="sxs-lookup"><span data-stu-id="bfc66-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bfc66-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc66-118">Authorization</span></span>  | <span data-ttu-id="bfc66-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfc66-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bfc66-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="bfc66-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfc66-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="bfc66-124">Request body</span></span>
<span data-ttu-id="bfc66-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfc66-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bfc66-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bfc66-126">Parameter</span></span>    | <span data-ttu-id="bfc66-127">Type</span><span class="sxs-lookup"><span data-stu-id="bfc66-127">Type</span></span>   |<span data-ttu-id="bfc66-128">説明</span><span class="sxs-lookup"><span data-stu-id="bfc66-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfc66-129">height</span><span class="sxs-lookup"><span data-stu-id="bfc66-129">height</span></span>|<span data-ttu-id="bfc66-130">number</span><span class="sxs-lookup"><span data-stu-id="bfc66-130">number</span></span>|<span data-ttu-id="bfc66-p104">省略可能。結果の画像の希望する高さ。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="bfc66-133">width</span><span class="sxs-lookup"><span data-stu-id="bfc66-133">width</span></span>|<span data-ttu-id="bfc66-134">number</span><span class="sxs-lookup"><span data-stu-id="bfc66-134">number</span></span>|<span data-ttu-id="bfc66-p105">省略可能。結果の画像の希望する幅。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="bfc66-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="bfc66-137">fittingMode</span></span>|<span data-ttu-id="bfc66-138">string</span><span class="sxs-lookup"><span data-stu-id="bfc66-138">string</span></span>|<span data-ttu-id="bfc66-p106">省略可能。指定したディメンションに合わせてグラフを拡大または縮小するために使用するメソッド (高さと幅の両方が設定されている場合)。使用可能な値: `Fit`、`FitAndCenter`、`Fill`。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p106">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="bfc66-142">応答</span><span class="sxs-lookup"><span data-stu-id="bfc66-142">Response</span></span>

<span data-ttu-id="bfc66-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で base-64 画像 string を返します。</span><span class="sxs-lookup"><span data-stu-id="bfc66-143">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfc66-144">例</span><span class="sxs-lookup"><span data-stu-id="bfc66-144">Example</span></span>
<span data-ttu-id="bfc66-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bfc66-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bfc66-146">要求</span><span class="sxs-lookup"><span data-stu-id="bfc66-146">Request</span></span>
<span data-ttu-id="bfc66-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bfc66-147">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="bfc66-148">応答</span><span class="sxs-lookup"><span data-stu-id="bfc66-148">Response</span></span>
<span data-ttu-id="bfc66-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bfc66-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="bfc66-152">使用方法</span><span class="sxs-lookup"><span data-stu-id="bfc66-152">Usage</span></span>

<span data-ttu-id="bfc66-153">HTML イメージ タグ: `<img src="data:image/png;base64,{base-64 chart image string}/>` 内の Base-64 文字列を表示できます。</span><span class="sxs-lookup"><span data-stu-id="bfc66-153">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="bfc66-154">既定の動作には、`Image(width=0,height=0,fittingMode='fit')` を使用します。</span><span class="sxs-lookup"><span data-stu-id="bfc66-154">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="bfc66-155">既定のパラメーターで返されるグラフ イメージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bfc66-155">Here is an example of a chart image returned with the default parameters.</span></span>

![既定値の高さと幅の Excel グラフのイメージです。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="bfc66-157">イメージの表示をカスタマイズする場合は、高さ、幅、自動調整モードを指定します。</span><span class="sxs-lookup"><span data-stu-id="bfc66-157">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="bfc66-158">これらのパラメーターを使用してグラフ イメージを取得する場合、どのように表示されるかを次に示します。`Image(width=500,height=500,fittingMode='Fill')`。</span><span class="sxs-lookup"><span data-stu-id="bfc66-158">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
