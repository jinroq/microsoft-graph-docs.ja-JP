# <a name="update-chartaxistitle"></a><span data-ttu-id="471cf-101">Update chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="471cf-101">Update chartaxistitle</span></span>

<span data-ttu-id="471cf-102">chartaxistitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="471cf-102">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="471cf-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="471cf-103">Permissions</span></span>
<span data-ttu-id="471cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="471cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="471cf-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="471cf-106">Permission type</span></span>      | <span data-ttu-id="471cf-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="471cf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="471cf-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="471cf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="471cf-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="471cf-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="471cf-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="471cf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="471cf-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="471cf-111">Not supported.</span></span>    |
|<span data-ttu-id="471cf-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="471cf-112">Application</span></span> | <span data-ttu-id="471cf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="471cf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="471cf-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="471cf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="471cf-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="471cf-115">Optional request headers</span></span>
| <span data-ttu-id="471cf-116">名前</span><span class="sxs-lookup"><span data-stu-id="471cf-116">Name</span></span>       | <span data-ttu-id="471cf-117">説明</span><span class="sxs-lookup"><span data-stu-id="471cf-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="471cf-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="471cf-118">Authorization</span></span>  | <span data-ttu-id="471cf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="471cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="471cf-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="471cf-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="471cf-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="471cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="471cf-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="471cf-124">Request body</span></span>
<span data-ttu-id="471cf-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="471cf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="471cf-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="471cf-128">Property</span></span>     | <span data-ttu-id="471cf-129">型</span><span class="sxs-lookup"><span data-stu-id="471cf-129">Type</span></span>   |<span data-ttu-id="471cf-130">説明</span><span class="sxs-lookup"><span data-stu-id="471cf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="471cf-131">text</span><span class="sxs-lookup"><span data-stu-id="471cf-131">text</span></span>|<span data-ttu-id="471cf-132">string</span><span class="sxs-lookup"><span data-stu-id="471cf-132">string</span></span>|<span data-ttu-id="471cf-133">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="471cf-133">Represents the axis title.</span></span>|
|<span data-ttu-id="471cf-134">visible</span><span class="sxs-lookup"><span data-stu-id="471cf-134">visible</span></span>|<span data-ttu-id="471cf-135">boolean</span><span class="sxs-lookup"><span data-stu-id="471cf-135">boolean</span></span>|<span data-ttu-id="471cf-136">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="471cf-136">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="471cf-137">応答</span><span class="sxs-lookup"><span data-stu-id="471cf-137">Response</span></span>

<span data-ttu-id="471cf-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartAxisTitle](../resources/chartaxistitle.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="471cf-138">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="471cf-139">例</span><span class="sxs-lookup"><span data-stu-id="471cf-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="471cf-140">要求</span><span class="sxs-lookup"><span data-stu-id="471cf-140">Request</span></span>
<span data-ttu-id="471cf-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="471cf-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="471cf-142">応答</span><span class="sxs-lookup"><span data-stu-id="471cf-142">Response</span></span>
<span data-ttu-id="471cf-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="471cf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->