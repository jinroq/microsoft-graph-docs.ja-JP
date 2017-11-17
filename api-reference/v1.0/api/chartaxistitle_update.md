# <a name="update-chartaxistitle"></a><span data-ttu-id="cf096-101">Update chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="cf096-101">Update chartaxistitle</span></span>

<span data-ttu-id="cf096-102">chartaxistitle オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf096-102">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf096-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cf096-103">Permissions</span></span>
<span data-ttu-id="cf096-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf096-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf096-106">Permission type</span></span>      | <span data-ttu-id="cf096-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf096-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf096-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf096-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cf096-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf096-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf096-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf096-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf096-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf096-111">Not supported.</span></span>    |
|<span data-ttu-id="cf096-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf096-112">Application</span></span> | <span data-ttu-id="cf096-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf096-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf096-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf096-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="cf096-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf096-115">Optional request headers</span></span>
| <span data-ttu-id="cf096-116">名前</span><span class="sxs-lookup"><span data-stu-id="cf096-116">Name</span></span>       | <span data-ttu-id="cf096-117">説明</span><span class="sxs-lookup"><span data-stu-id="cf096-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cf096-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf096-118">Authorization</span></span>  | <span data-ttu-id="cf096-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cf096-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf096-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf096-121">Request body</span></span>
<span data-ttu-id="cf096-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cf096-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf096-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf096-125">Property</span></span>     | <span data-ttu-id="cf096-126">型</span><span class="sxs-lookup"><span data-stu-id="cf096-126">Type</span></span>   |<span data-ttu-id="cf096-127">説明</span><span class="sxs-lookup"><span data-stu-id="cf096-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf096-128">text</span><span class="sxs-lookup"><span data-stu-id="cf096-128">text</span></span>|<span data-ttu-id="cf096-129">string</span><span class="sxs-lookup"><span data-stu-id="cf096-129">string</span></span>|<span data-ttu-id="cf096-130">軸タイトルを表します。</span><span class="sxs-lookup"><span data-stu-id="cf096-130">Represents the axis title.</span></span>|
|<span data-ttu-id="cf096-131">visible</span><span class="sxs-lookup"><span data-stu-id="cf096-131">visible</span></span>|<span data-ttu-id="cf096-132">boolean</span><span class="sxs-lookup"><span data-stu-id="cf096-132">boolean</span></span>|<span data-ttu-id="cf096-133">軸のタイトルの表示/非表示を指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="cf096-133">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="cf096-134">応答</span><span class="sxs-lookup"><span data-stu-id="cf096-134">Response</span></span>

<span data-ttu-id="cf096-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [ChartAxisTitle](../resources/chartaxistitle.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf096-135">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf096-136">例</span><span class="sxs-lookup"><span data-stu-id="cf096-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf096-137">要求</span><span class="sxs-lookup"><span data-stu-id="cf096-137">Request</span></span>
<span data-ttu-id="cf096-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf096-138">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="cf096-139">応答</span><span class="sxs-lookup"><span data-stu-id="cf096-139">Response</span></span>
<span data-ttu-id="cf096-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf096-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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