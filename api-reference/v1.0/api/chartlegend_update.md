# <a name="update-chartlegend"></a><span data-ttu-id="9f161-101">Update chartlegend</span><span class="sxs-lookup"><span data-stu-id="9f161-101">Update chartlegend</span></span>

<span data-ttu-id="9f161-102">chartlegend オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f161-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f161-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f161-103">Permissions</span></span>
<span data-ttu-id="9f161-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f161-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f161-106">Permission type</span></span>      | <span data-ttu-id="9f161-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f161-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f161-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f161-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9f161-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f161-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f161-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f161-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f161-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f161-111">Not supported.</span></span>    |
|<span data-ttu-id="9f161-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f161-112">Application</span></span> | <span data-ttu-id="9f161-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f161-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f161-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f161-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="9f161-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f161-115">Optional request headers</span></span>
| <span data-ttu-id="9f161-116">名前</span><span class="sxs-lookup"><span data-stu-id="9f161-116">Name</span></span>       | <span data-ttu-id="9f161-117">説明</span><span class="sxs-lookup"><span data-stu-id="9f161-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9f161-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f161-118">Authorization</span></span>  | <span data-ttu-id="9f161-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9f161-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f161-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f161-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f161-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9f161-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f161-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f161-124">Request body</span></span>
<span data-ttu-id="9f161-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9f161-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f161-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f161-128">Property</span></span>     | <span data-ttu-id="9f161-129">型</span><span class="sxs-lookup"><span data-stu-id="9f161-129">Type</span></span>   |<span data-ttu-id="9f161-130">説明</span><span class="sxs-lookup"><span data-stu-id="9f161-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f161-131">overlay</span><span class="sxs-lookup"><span data-stu-id="9f161-131">overlay</span></span>|<span data-ttu-id="9f161-132">boolean</span><span class="sxs-lookup"><span data-stu-id="9f161-132">boolean</span></span>|<span data-ttu-id="9f161-133">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="9f161-133">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="9f161-134">position</span><span class="sxs-lookup"><span data-stu-id="9f161-134">position</span></span>|<span data-ttu-id="9f161-135">string</span><span class="sxs-lookup"><span data-stu-id="9f161-135">string</span></span>|<span data-ttu-id="9f161-p105">グラフの凡例の位置を表します。可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。</span><span class="sxs-lookup"><span data-stu-id="9f161-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="9f161-138">visible</span><span class="sxs-lookup"><span data-stu-id="9f161-138">visible</span></span>|<span data-ttu-id="9f161-139">boolean</span><span class="sxs-lookup"><span data-stu-id="9f161-139">boolean</span></span>|<span data-ttu-id="9f161-140">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="9f161-140">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="9f161-141">応答</span><span class="sxs-lookup"><span data-stu-id="9f161-141">Response</span></span>

<span data-ttu-id="9f161-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartLegend](../resources/chartlegend.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f161-142">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f161-143">例</span><span class="sxs-lookup"><span data-stu-id="9f161-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f161-144">要求</span><span class="sxs-lookup"><span data-stu-id="9f161-144">Request</span></span>
<span data-ttu-id="9f161-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f161-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="9f161-146">応答</span><span class="sxs-lookup"><span data-stu-id="9f161-146">Response</span></span>
<span data-ttu-id="9f161-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f161-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->