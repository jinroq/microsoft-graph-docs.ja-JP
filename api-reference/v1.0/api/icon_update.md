# <a name="update-icon"></a><span data-ttu-id="c4d5c-101">アイコンを更新する</span><span class="sxs-lookup"><span data-stu-id="c4d5c-101">Update icon</span></span>

<span data-ttu-id="c4d5c-102">アイコン オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-102">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4d5c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4d5c-103">Permissions</span></span>
<span data-ttu-id="c4d5c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c4d5c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4d5c-106">Permission type</span></span>      | <span data-ttu-id="c4d5c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4d5c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c4d5c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4d5c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c4d5c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4d5c-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="c4d5c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4d5c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4d5c-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-111">Not supported.</span></span>    | 
|<span data-ttu-id="c4d5c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4d5c-112">Application</span></span> | <span data-ttu-id="c4d5c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c4d5c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4d5c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="c4d5c-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4d5c-115">Optional request headers</span></span>
| <span data-ttu-id="c4d5c-116">名前</span><span class="sxs-lookup"><span data-stu-id="c4d5c-116">Name</span></span>       | <span data-ttu-id="c4d5c-117">説明</span><span class="sxs-lookup"><span data-stu-id="c4d5c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c4d5c-118">承認</span><span class="sxs-lookup"><span data-stu-id="c4d5c-118">Authorization</span></span>  | <span data-ttu-id="c4d5c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c4d5c-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4d5c-121">Request body</span></span>
<span data-ttu-id="c4d5c-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c4d5c-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4d5c-125">Property</span></span>     | <span data-ttu-id="c4d5c-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="c4d5c-126">Type</span></span>   |<span data-ttu-id="c4d5c-127">説明</span><span class="sxs-lookup"><span data-stu-id="c4d5c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4d5c-128">index</span><span class="sxs-lookup"><span data-stu-id="c4d5c-128">index</span></span>|<span data-ttu-id="c4d5c-129">int</span><span class="sxs-lookup"><span data-stu-id="c4d5c-129">int</span></span>|<span data-ttu-id="c4d5c-130">指定したセット内のアイコンのインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-130">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="c4d5c-131">set</span><span class="sxs-lookup"><span data-stu-id="c4d5c-131">set</span></span>|<span data-ttu-id="c4d5c-132">string</span><span class="sxs-lookup"><span data-stu-id="c4d5c-132">string</span></span>|<span data-ttu-id="c4d5c-133">部分的にアイコンを含むセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-133">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="c4d5c-134">可能な値は、 `Invalid`、 `ThreeArrows`、 `ThreeArrowsGray`、 `ThreeFlags`、 `ThreeTrafficLights1`、 `ThreeTrafficLights2`、 `ThreeSigns`、 `ThreeSymbols`、 `ThreeSymbols2`、 `FourArrows`、 `FourArrowsGray`、 `FourRedToBlack`、 `FourRating`、 `FourTrafficLights`、 `FiveArrows`、 `FiveArrowsGray`、 `FiveRating`、 `FiveQuarters`、 `ThreeStars`, `ThreeTriangles`, `FiveBoxes` です。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-134">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="c4d5c-135">応答</span><span class="sxs-lookup"><span data-stu-id="c4d5c-135">Response</span></span>

<span data-ttu-id="c4d5c-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アイコン](../resources/icon.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-136">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4d5c-137">例</span><span class="sxs-lookup"><span data-stu-id="c4d5c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4d5c-138">要求</span><span class="sxs-lookup"><span data-stu-id="c4d5c-138">Request</span></span>
<span data-ttu-id="c4d5c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="c4d5c-140">応答</span><span class="sxs-lookup"><span data-stu-id="c4d5c-140">Response</span></span>
<span data-ttu-id="c4d5c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4d5c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->