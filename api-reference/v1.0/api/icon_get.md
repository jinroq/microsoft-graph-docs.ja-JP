# <a name="get-icon"></a><span data-ttu-id="c8ec3-101">アイコンを取得する</span><span class="sxs-lookup"><span data-stu-id="c8ec3-101">Get Icon</span></span>

<span data-ttu-id="c8ec3-102">アイコン オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-102">Retrieve the properties and relationships of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8ec3-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8ec3-103">Prerequisites</span></span>
<span data-ttu-id="c8ec3-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="c8ec3-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8ec3-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="c8ec3-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8ec3-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8ec3-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8ec3-107">Optional query parameters</span></span>
<span data-ttu-id="c8ec3-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8ec3-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8ec3-109">Request headers</span></span>
| <span data-ttu-id="c8ec3-110">名前</span><span class="sxs-lookup"><span data-stu-id="c8ec3-110">Name</span></span>      |<span data-ttu-id="c8ec3-111">説明</span><span class="sxs-lookup"><span data-stu-id="c8ec3-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8ec3-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8ec3-112">Authorization</span></span>  | <span data-ttu-id="c8ec3-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8ec3-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8ec3-115">Request body</span></span>
<span data-ttu-id="c8ec3-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8ec3-117">応答</span><span class="sxs-lookup"><span data-stu-id="c8ec3-117">Response</span></span>

<span data-ttu-id="c8ec3-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アイコン](../resources/icon.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-118">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8ec3-119">例</span><span class="sxs-lookup"><span data-stu-id="c8ec3-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8ec3-120">要求</span><span class="sxs-lookup"><span data-stu-id="c8ec3-120">Request</span></span>
<span data-ttu-id="c8ec3-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="c8ec3-122">応答</span><span class="sxs-lookup"><span data-stu-id="c8ec3-122">Response</span></span>
<span data-ttu-id="c8ec3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8ec3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
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
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->