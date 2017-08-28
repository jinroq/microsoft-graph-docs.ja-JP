# <a name="get-formatprotection"></a><span data-ttu-id="12e33-101">FormatProtection の取得</span><span class="sxs-lookup"><span data-stu-id="12e33-101">Get FormatProtection</span></span>

<span data-ttu-id="12e33-102">formatprotection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="12e33-102">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12e33-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="12e33-103">Prerequisites</span></span>
<span data-ttu-id="12e33-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="12e33-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="12e33-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12e33-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="12e33-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12e33-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12e33-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="12e33-107">Optional query parameters</span></span>
<span data-ttu-id="12e33-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="12e33-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12e33-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12e33-109">Request headers</span></span>
| <span data-ttu-id="12e33-110">名前</span><span class="sxs-lookup"><span data-stu-id="12e33-110">Name</span></span>      |<span data-ttu-id="12e33-111">説明</span><span class="sxs-lookup"><span data-stu-id="12e33-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12e33-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="12e33-112">Authorization</span></span>  | <span data-ttu-id="12e33-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12e33-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12e33-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="12e33-115">Request body</span></span>
<span data-ttu-id="12e33-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12e33-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12e33-117">応答</span><span class="sxs-lookup"><span data-stu-id="12e33-117">Response</span></span>

<span data-ttu-id="12e33-118">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [FormatProtection](../resources/formatprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12e33-118">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12e33-119">例</span><span class="sxs-lookup"><span data-stu-id="12e33-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12e33-120">要求</span><span class="sxs-lookup"><span data-stu-id="12e33-120">Request</span></span>
<span data-ttu-id="12e33-121">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12e33-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="12e33-122">応答</span><span class="sxs-lookup"><span data-stu-id="12e33-122">Response</span></span>
<span data-ttu-id="12e33-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12e33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->