# <a name="create-rangeborder"></a><span data-ttu-id="1cd11-101">RangeBorder を作成する</span><span class="sxs-lookup"><span data-stu-id="1cd11-101">Create RangeBorder</span></span>

<span data-ttu-id="1cd11-102">この API を使用して、新しい RangeBorder を作成します。</span><span class="sxs-lookup"><span data-stu-id="1cd11-102">Use this API to create a new RangeBorder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cd11-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="1cd11-103">Prerequisites</span></span>
<span data-ttu-id="1cd11-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1cd11-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="1cd11-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1cd11-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="1cd11-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1cd11-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="1cd11-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cd11-107">Request headers</span></span>
| <span data-ttu-id="1cd11-108">名前</span><span class="sxs-lookup"><span data-stu-id="1cd11-108">Name</span></span>       | <span data-ttu-id="1cd11-109">説明</span><span class="sxs-lookup"><span data-stu-id="1cd11-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1cd11-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cd11-110">Authorization</span></span>  | <span data-ttu-id="1cd11-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1cd11-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1cd11-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="1cd11-113">Request body</span></span>
<span data-ttu-id="1cd11-114">要求本文で、[RangeBorder](../resources/rangeborder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd11-114">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1cd11-115">応答</span><span class="sxs-lookup"><span data-stu-id="1cd11-115">Response</span></span>

<span data-ttu-id="1cd11-116">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [RangeBorder](../resources/rangeborder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1cd11-116">If successful, this method returns `201, Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd11-117">例</span><span class="sxs-lookup"><span data-stu-id="1cd11-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cd11-118">要求</span><span class="sxs-lookup"><span data-stu-id="1cd11-118">Request</span></span>
<span data-ttu-id="1cd11-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1cd11-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
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
<span data-ttu-id="1cd11-120">要求本文で、[RangeBorder](../resources/rangeborder.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cd11-120">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1cd11-121">応答</span><span class="sxs-lookup"><span data-stu-id="1cd11-121">Response</span></span>
<span data-ttu-id="1cd11-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1cd11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->