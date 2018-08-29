# <a name="chartseriescollection-itemat"></a><span data-ttu-id="e0dcf-101">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="e0dcf-101">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="e0dcf-102">コレクション内の位置に基づいてデータ系列を取得します。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-102">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="e0dcf-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e0dcf-103">Permissions</span></span>
<span data-ttu-id="e0dcf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0dcf-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0dcf-106">Permission type</span></span>      | <span data-ttu-id="e0dcf-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0dcf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0dcf-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0dcf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e0dcf-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0dcf-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0dcf-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0dcf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0dcf-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-111">Not supported.</span></span>    |
|<span data-ttu-id="e0dcf-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0dcf-112">Application</span></span> | <span data-ttu-id="e0dcf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0dcf-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0dcf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="e0dcf-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0dcf-115">Request headers</span></span>
| <span data-ttu-id="e0dcf-116">名前</span><span class="sxs-lookup"><span data-stu-id="e0dcf-116">Name</span></span>       | <span data-ttu-id="e0dcf-117">説明</span><span class="sxs-lookup"><span data-stu-id="e0dcf-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0dcf-118">承認</span><span class="sxs-lookup"><span data-stu-id="e0dcf-118">Authorization</span></span>  | <span data-ttu-id="e0dcf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0dcf-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0dcf-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0dcf-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0dcf-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0dcf-124">Request body</span></span>
<span data-ttu-id="e0dcf-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0dcf-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e0dcf-126">Parameter</span></span>    | <span data-ttu-id="e0dcf-127">型</span><span class="sxs-lookup"><span data-stu-id="e0dcf-127">Type</span></span>   |<span data-ttu-id="e0dcf-128">説明</span><span class="sxs-lookup"><span data-stu-id="e0dcf-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0dcf-129">インデックス</span><span class="sxs-lookup"><span data-stu-id="e0dcf-129">index</span></span>|<span data-ttu-id="e0dcf-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e0dcf-130">Int32</span></span>|<span data-ttu-id="e0dcf-p104">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e0dcf-133">応答</span><span class="sxs-lookup"><span data-stu-id="e0dcf-133">Response</span></span>

<span data-ttu-id="e0dcf-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[WorkbookChartSeries](../resources/chartseries.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-134">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0dcf-135">例</span><span class="sxs-lookup"><span data-stu-id="e0dcf-135">Example</span></span>
<span data-ttu-id="e0dcf-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0dcf-137">要求</span><span class="sxs-lookup"><span data-stu-id="e0dcf-137">Request</span></span>
<span data-ttu-id="e0dcf-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="e0dcf-139">応答</span><span class="sxs-lookup"><span data-stu-id="e0dcf-139">Response</span></span>
<span data-ttu-id="e0dcf-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0dcf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->