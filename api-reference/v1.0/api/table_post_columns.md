# <a name="create-tablecolumn"></a><span data-ttu-id="b1638-101">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="b1638-101">Create TableColumn</span></span>

<span data-ttu-id="b1638-102">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="b1638-102">Use this API to create a new TableColumn.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1638-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1638-103">Prerequisites</span></span>
<span data-ttu-id="b1638-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b1638-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="b1638-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1638-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="b1638-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1638-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="b1638-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1638-107">Request headers</span></span>
| <span data-ttu-id="b1638-108">名前</span><span class="sxs-lookup"><span data-stu-id="b1638-108">Name</span></span>       | <span data-ttu-id="b1638-109">説明</span><span class="sxs-lookup"><span data-stu-id="b1638-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b1638-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1638-110">Authorization</span></span>  | <span data-ttu-id="b1638-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1638-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b1638-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1638-113">Request body</span></span>
<span data-ttu-id="b1638-114">要求本文で、[TableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1638-114">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1638-115">応答</span><span class="sxs-lookup"><span data-stu-id="b1638-115">Response</span></span>

<span data-ttu-id="b1638-116">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1638-116">If successful, this method returns `201, Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1638-117">例</span><span class="sxs-lookup"><span data-stu-id="b1638-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1638-118">要求</span><span class="sxs-lookup"><span data-stu-id="b1638-118">Request</span></span>
<span data-ttu-id="b1638-119">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1638-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="b1638-120">要求本文で、[TableColumn](../resources/tablecolumn.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1638-120">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b1638-121">応答</span><span class="sxs-lookup"><span data-stu-id="b1638-121">Response</span></span>
<span data-ttu-id="b1638-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1638-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->