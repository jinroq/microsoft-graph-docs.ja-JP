# <a name="create-chartseries"></a><span data-ttu-id="6977d-101">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="6977d-101">Create ChartSeries</span></span>

<span data-ttu-id="6977d-102">この API を使用して、新しい ChartSeries を作成します。</span><span class="sxs-lookup"><span data-stu-id="6977d-102">Use this API to create a new ChartSeries.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6977d-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="6977d-103">Prerequisites</span></span>
<span data-ttu-id="6977d-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6977d-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="6977d-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6977d-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="6977d-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6977d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="6977d-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6977d-107">Request headers</span></span>
| <span data-ttu-id="6977d-108">名前</span><span class="sxs-lookup"><span data-stu-id="6977d-108">Name</span></span>       | <span data-ttu-id="6977d-109">説明</span><span class="sxs-lookup"><span data-stu-id="6977d-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6977d-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="6977d-110">Authorization</span></span>  | <span data-ttu-id="6977d-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6977d-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6977d-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="6977d-113">Request body</span></span>
<span data-ttu-id="6977d-114">要求本文で、[ChartSeries](../resources/chartseries.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6977d-114">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6977d-115">応答</span><span class="sxs-lookup"><span data-stu-id="6977d-115">Response</span></span>

<span data-ttu-id="6977d-116">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [ChartSeries](../resources/chartseries.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6977d-116">If successful, this method returns `201, Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6977d-117">例</span><span class="sxs-lookup"><span data-stu-id="6977d-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6977d-118">要求</span><span class="sxs-lookup"><span data-stu-id="6977d-118">Request</span></span>
<span data-ttu-id="6977d-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6977d-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="6977d-120">要求本文で、[ChartSeries](../resources/chartseries.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6977d-120">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6977d-121">応答</span><span class="sxs-lookup"><span data-stu-id="6977d-121">Response</span></span>
<span data-ttu-id="6977d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6977d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->