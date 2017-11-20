# <a name="chart-setdata"></a><span data-ttu-id="a9ba4-101">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="a9ba4-101">Chart: setData</span></span>

<span data-ttu-id="a9ba4-102">グラフのソース データをリセットします。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-102">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9ba4-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9ba4-103">Permissions</span></span>
<span data-ttu-id="a9ba4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9ba4-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9ba4-106">Permission type</span></span>      | <span data-ttu-id="a9ba4-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9ba4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9ba4-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9ba4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a9ba4-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9ba4-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9ba4-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9ba4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ba4-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-111">Not supported.</span></span>    |
|<span data-ttu-id="a9ba4-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9ba4-112">Application</span></span> | <span data-ttu-id="a9ba4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ba4-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9ba4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="a9ba4-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9ba4-115">Request headers</span></span>
| <span data-ttu-id="a9ba4-116">名前</span><span class="sxs-lookup"><span data-stu-id="a9ba4-116">Name</span></span>       | <span data-ttu-id="a9ba4-117">説明</span><span class="sxs-lookup"><span data-stu-id="a9ba4-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a9ba4-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9ba4-118">Authorization</span></span>  | <span data-ttu-id="a9ba4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9ba4-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9ba4-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9ba4-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9ba4-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9ba4-124">Request body</span></span>
<span data-ttu-id="a9ba4-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9ba4-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a9ba4-126">Parameter</span></span>    | <span data-ttu-id="a9ba4-127">Type</span><span class="sxs-lookup"><span data-stu-id="a9ba4-127">Type</span></span>   |<span data-ttu-id="a9ba4-128">説明</span><span class="sxs-lookup"><span data-stu-id="a9ba4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9ba4-129">sourceData</span><span class="sxs-lookup"><span data-stu-id="a9ba4-129">sourceData</span></span>|<span data-ttu-id="a9ba4-130">string</span><span class="sxs-lookup"><span data-stu-id="a9ba4-130">string</span></span>|<span data-ttu-id="a9ba4-131">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-131">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="a9ba4-132">seriesBy</span><span class="sxs-lookup"><span data-stu-id="a9ba4-132">seriesBy</span></span>|<span data-ttu-id="a9ba4-133">string</span><span class="sxs-lookup"><span data-stu-id="a9ba4-133">string</span></span>|<span data-ttu-id="a9ba4-p104">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。次のいずれかを指定できます。自動 (既定)、行、列。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="a9ba4-138">応答</span><span class="sxs-lookup"><span data-stu-id="a9ba4-138">Response</span></span>

<span data-ttu-id="a9ba4-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ba4-141">例</span><span class="sxs-lookup"><span data-stu-id="a9ba4-141">Example</span></span>
<span data-ttu-id="a9ba4-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a9ba4-143">要求</span><span class="sxs-lookup"><span data-stu-id="a9ba4-143">Request</span></span>
<span data-ttu-id="a9ba4-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="a9ba4-145">応答</span><span class="sxs-lookup"><span data-stu-id="a9ba4-145">Response</span></span>
<span data-ttu-id="a9ba4-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a9ba4-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->