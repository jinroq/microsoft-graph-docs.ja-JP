# <a name="list-tablecollection"></a><span data-ttu-id="b9a3f-101">TableCollection の一覧表示</span><span class="sxs-lookup"><span data-stu-id="b9a3f-101">List TableCollection</span></span>

<span data-ttu-id="b9a3f-102">テーブル オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-102">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9a3f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b9a3f-103">Permissions</span></span>
<span data-ttu-id="b9a3f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9a3f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9a3f-106">Permission type</span></span>      | <span data-ttu-id="b9a3f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9a3f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a3f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a3f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a3f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a3f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9a3f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a3f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a3f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-111">Not supported.</span></span>    |
|<span data-ttu-id="b9a3f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9a3f-112">Application</span></span> | <span data-ttu-id="b9a3f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a3f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9a3f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9a3f-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9a3f-115">Optional query parameters</span></span>
<span data-ttu-id="b9a3f-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9a3f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9a3f-117">Request headers</span></span>
| <span data-ttu-id="b9a3f-118">名前</span><span class="sxs-lookup"><span data-stu-id="b9a3f-118">Name</span></span>      |<span data-ttu-id="b9a3f-119">説明</span><span class="sxs-lookup"><span data-stu-id="b9a3f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9a3f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9a3f-120">Authorization</span></span>  | <span data-ttu-id="b9a3f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a3f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9a3f-123">Request body</span></span>
<span data-ttu-id="b9a3f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a3f-125">応答</span><span class="sxs-lookup"><span data-stu-id="b9a3f-125">Response</span></span>

<span data-ttu-id="b9a3f-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Table](../resources/table.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-126">If successful, this method returns a `200 OK` response code and collection of [Table](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9a3f-127">例</span><span class="sxs-lookup"><span data-stu-id="b9a3f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9a3f-128">要求</span><span class="sxs-lookup"><span data-stu-id="b9a3f-128">Request</span></span>
<span data-ttu-id="b9a3f-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="b9a3f-130">応答</span><span class="sxs-lookup"><span data-stu-id="b9a3f-130">Response</span></span>
<span data-ttu-id="b9a3f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
> <span data-ttu-id="b9a3f-134">**注:** [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) クエリ パラメーターを使用して、多数のテーブルをページングします。</span><span class="sxs-lookup"><span data-stu-id="b9a3f-134">**Note:** Use the [$top](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/en-us/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="b9a3f-135">例:</span><span class="sxs-lookup"><span data-stu-id="b9a3f-135">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
