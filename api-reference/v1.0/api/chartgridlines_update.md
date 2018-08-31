# <a name="update-chartgridlines"></a><span data-ttu-id="369f2-101">Update chartgridlines</span><span class="sxs-lookup"><span data-stu-id="369f2-101">Update chartgridlines</span></span>

<span data-ttu-id="369f2-102">chartgridlines オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="369f2-102">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="369f2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="369f2-103">Permissions</span></span>
<span data-ttu-id="369f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="369f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="369f2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="369f2-106">Permission type</span></span>      | <span data-ttu-id="369f2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="369f2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="369f2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="369f2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="369f2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="369f2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="369f2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="369f2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="369f2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369f2-111">Not supported.</span></span>    |
|<span data-ttu-id="369f2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="369f2-112">Application</span></span> | <span data-ttu-id="369f2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369f2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="369f2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="369f2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="369f2-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="369f2-115">Request headers</span></span>
| <span data-ttu-id="369f2-116">名前</span><span class="sxs-lookup"><span data-stu-id="369f2-116">Name</span></span>       | <span data-ttu-id="369f2-117">説明</span><span class="sxs-lookup"><span data-stu-id="369f2-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="369f2-118">承認</span><span class="sxs-lookup"><span data-stu-id="369f2-118">Authorization</span></span>  | <span data-ttu-id="369f2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="369f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="369f2-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="369f2-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="369f2-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="369f2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="369f2-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="369f2-124">Request body</span></span>
<span data-ttu-id="369f2-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="369f2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="369f2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="369f2-128">Property</span></span>     | <span data-ttu-id="369f2-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="369f2-129">Type</span></span>   |<span data-ttu-id="369f2-130">説明</span><span class="sxs-lookup"><span data-stu-id="369f2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="369f2-131">visible</span><span class="sxs-lookup"><span data-stu-id="369f2-131">visible</span></span>|<span data-ttu-id="369f2-132">boolean</span><span class="sxs-lookup"><span data-stu-id="369f2-132">boolean</span></span>|<span data-ttu-id="369f2-133">軸の目盛線を表示するか非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="369f2-133">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="369f2-134">応答</span><span class="sxs-lookup"><span data-stu-id="369f2-134">Response</span></span>

<span data-ttu-id="369f2-135">成功した場合、このメソッドは `200 OK` 応答コードを返し、応答本文で [WorkbookChartGridlines](../resources/chartgridlines.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="369f2-135">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="369f2-136">例</span><span class="sxs-lookup"><span data-stu-id="369f2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="369f2-137">要求</span><span class="sxs-lookup"><span data-stu-id="369f2-137">Request</span></span>
<span data-ttu-id="369f2-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="369f2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="369f2-139">応答</span><span class="sxs-lookup"><span data-stu-id="369f2-139">Response</span></span>
<span data-ttu-id="369f2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="369f2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->