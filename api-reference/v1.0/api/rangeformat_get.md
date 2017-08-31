# <a name="get-rangeformat"></a><span data-ttu-id="705b9-101">RangeFormat を取得する</span><span class="sxs-lookup"><span data-stu-id="705b9-101">Get RangeFormat</span></span>

<span data-ttu-id="705b9-102">rangeformat オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="705b9-102">Retrieve the properties and relationships of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="705b9-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="705b9-103">Permissions</span></span>
<span data-ttu-id="705b9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="705b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="705b9-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="705b9-106">Permission type</span></span>      | <span data-ttu-id="705b9-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="705b9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="705b9-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="705b9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="705b9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="705b9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="705b9-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="705b9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="705b9-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="705b9-111">Not supported.</span></span>    |
|<span data-ttu-id="705b9-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="705b9-112">Application</span></span> | <span data-ttu-id="705b9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="705b9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="705b9-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="705b9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format
GET /workbook/worksheets/{id|name}/range(<address>)/format
GET /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-query-parameters"></a><span data-ttu-id="705b9-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="705b9-115">Optional query parameters</span></span>
<span data-ttu-id="705b9-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="705b9-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="705b9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="705b9-117">Request headers</span></span>
| <span data-ttu-id="705b9-118">名前</span><span class="sxs-lookup"><span data-stu-id="705b9-118">Name</span></span>      |<span data-ttu-id="705b9-119">説明</span><span class="sxs-lookup"><span data-stu-id="705b9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="705b9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="705b9-120">Authorization</span></span>  | <span data-ttu-id="705b9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="705b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="705b9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="705b9-123">Request body</span></span>
<span data-ttu-id="705b9-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="705b9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="705b9-125">応答</span><span class="sxs-lookup"><span data-stu-id="705b9-125">Response</span></span>

<span data-ttu-id="705b9-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [RangeFormat](../resources/rangeformat.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="705b9-126">If successful, this method returns a `200 OK` response code and [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="705b9-127">例</span><span class="sxs-lookup"><span data-stu-id="705b9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="705b9-128">要求</span><span class="sxs-lookup"><span data-stu-id="705b9-128">Request</span></span>
<span data-ttu-id="705b9-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="705b9-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rangeformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
```
##### <a name="response"></a><span data-ttu-id="705b9-130">応答</span><span class="sxs-lookup"><span data-stu-id="705b9-130">Response</span></span>
<span data-ttu-id="705b9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="705b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get RangeFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->