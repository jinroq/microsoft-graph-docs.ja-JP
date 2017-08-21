# <a name="create-chartpoints"></a><span data-ttu-id="8937b-101">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="8937b-101">Create ChartPoints</span></span>

<span data-ttu-id="8937b-102">この API を使用して、新しい ChartPoints を作成します。</span><span class="sxs-lookup"><span data-stu-id="8937b-102">Use this API to create a new ChartPoints.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8937b-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="8937b-103">Prerequisites</span></span>
<span data-ttu-id="8937b-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="8937b-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="8937b-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8937b-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="8937b-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8937b-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="8937b-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8937b-107">Request headers</span></span>
| <span data-ttu-id="8937b-108">名前</span><span class="sxs-lookup"><span data-stu-id="8937b-108">Name</span></span>       | <span data-ttu-id="8937b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8937b-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8937b-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="8937b-110">Authorization</span></span>  | <span data-ttu-id="8937b-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8937b-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8937b-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="8937b-113">Request body</span></span>
<span data-ttu-id="8937b-114">要求本文で、[ChartPoints](../resources/chartpoint.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8937b-114">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8937b-115">応答</span><span class="sxs-lookup"><span data-stu-id="8937b-115">Response</span></span>

<span data-ttu-id="8937b-116">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [ChartPoints](../resources/chartpoint.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8937b-116">If successful, this method returns `201, Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8937b-117">例</span><span class="sxs-lookup"><span data-stu-id="8937b-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8937b-118">要求</span><span class="sxs-lookup"><span data-stu-id="8937b-118">Request</span></span>
<span data-ttu-id="8937b-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8937b-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="8937b-120">要求本文で、[ChartPoints](../resources/chartpoint.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8937b-120">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8937b-121">応答</span><span class="sxs-lookup"><span data-stu-id="8937b-121">Response</span></span>
<span data-ttu-id="8937b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8937b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->