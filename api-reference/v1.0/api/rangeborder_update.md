# <a name="update-rangeborder"></a><span data-ttu-id="87825-101">rangeborder を更新する</span><span class="sxs-lookup"><span data-stu-id="87825-101">Update rangeborder</span></span>

<span data-ttu-id="87825-102">rangeborder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="87825-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87825-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87825-103">Permissions</span></span>
<span data-ttu-id="87825-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87825-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87825-106">Permission type</span></span>      | <span data-ttu-id="87825-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87825-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87825-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87825-108">Delegated (work or school account)</span></span> | <span data-ttu-id="87825-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87825-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87825-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87825-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87825-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87825-111">Not supported.</span></span>    |
|<span data-ttu-id="87825-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87825-112">Application</span></span> | <span data-ttu-id="87825-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87825-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87825-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87825-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="87825-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87825-115">Optional request headers</span></span>
| <span data-ttu-id="87825-116">名前</span><span class="sxs-lookup"><span data-stu-id="87825-116">Name</span></span>       | <span data-ttu-id="87825-117">説明</span><span class="sxs-lookup"><span data-stu-id="87825-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="87825-118">承認</span><span class="sxs-lookup"><span data-stu-id="87825-118">Authorization</span></span>  | <span data-ttu-id="87825-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87825-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87825-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87825-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="87825-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="87825-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87825-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="87825-124">Request body</span></span>
<span data-ttu-id="87825-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="87825-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="87825-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87825-128">Property</span></span>     | <span data-ttu-id="87825-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="87825-129">Type</span></span>   |<span data-ttu-id="87825-130">説明</span><span class="sxs-lookup"><span data-stu-id="87825-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87825-131">color</span><span class="sxs-lookup"><span data-stu-id="87825-131">color</span></span>|<span data-ttu-id="87825-132">文字列</span><span class="sxs-lookup"><span data-stu-id="87825-132">string</span></span>|<span data-ttu-id="87825-133">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="87825-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="87825-134">style</span><span class="sxs-lookup"><span data-stu-id="87825-134">style</span></span>|<span data-ttu-id="87825-135">string</span><span class="sxs-lookup"><span data-stu-id="87825-135">string</span></span>|<span data-ttu-id="87825-136">境界線の線のスタイルを指定する線のスタイルの定数の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="87825-136">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="87825-137">可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。</span><span class="sxs-lookup"><span data-stu-id="87825-137">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="87825-138">weight</span><span class="sxs-lookup"><span data-stu-id="87825-138">weight</span></span>|<span data-ttu-id="87825-139">string</span><span class="sxs-lookup"><span data-stu-id="87825-139">string</span></span>|<span data-ttu-id="87825-140">範囲周辺の罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="87825-140">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="87825-141">可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。</span><span class="sxs-lookup"><span data-stu-id="87825-141">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="87825-142">応答</span><span class="sxs-lookup"><span data-stu-id="87825-142">Response</span></span>

<span data-ttu-id="87825-143">成功した場合、このメソッドは `200 OK` 応答コードを返し、応答本文で [WorkbookRangeBorder](../resources/rangeborder.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="87825-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87825-144">例</span><span class="sxs-lookup"><span data-stu-id="87825-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87825-145">要求</span><span class="sxs-lookup"><span data-stu-id="87825-145">Request</span></span>
<span data-ttu-id="87825-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87825-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="87825-147">応答</span><span class="sxs-lookup"><span data-stu-id="87825-147">Response</span></span>
<span data-ttu-id="87825-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87825-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->