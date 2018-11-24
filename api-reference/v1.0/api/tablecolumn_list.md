# <a name="list-tablecolumncollection"></a><span data-ttu-id="87549-101">TableColumnCollection を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="87549-101">List TableColumnCollection</span></span>

<span data-ttu-id="87549-102">tablecolumn オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="87549-102">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="87549-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87549-103">Permissions</span></span>
<span data-ttu-id="87549-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87549-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87549-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87549-106">Permission type</span></span>      | <span data-ttu-id="87549-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87549-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87549-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87549-108">Delegated (work or school account)</span></span> | <span data-ttu-id="87549-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87549-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87549-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87549-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87549-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87549-111">Not supported.</span></span>    |
|<span data-ttu-id="87549-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87549-112">Application</span></span> | <span data-ttu-id="87549-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87549-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87549-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87549-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87549-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87549-115">Optional query parameters</span></span>
<span data-ttu-id="87549-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="87549-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87549-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87549-117">Request headers</span></span>
| <span data-ttu-id="87549-118">名前</span><span class="sxs-lookup"><span data-stu-id="87549-118">Name</span></span>      |<span data-ttu-id="87549-119">説明</span><span class="sxs-lookup"><span data-stu-id="87549-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87549-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="87549-120">Authorization</span></span>  | <span data-ttu-id="87549-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87549-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87549-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87549-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="87549-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="87549-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87549-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="87549-126">Request body</span></span>
<span data-ttu-id="87549-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87549-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87549-128">応答</span><span class="sxs-lookup"><span data-stu-id="87549-128">Response</span></span>

<span data-ttu-id="87549-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="87549-129">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87549-130">例</span><span class="sxs-lookup"><span data-stu-id="87549-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87549-131">要求</span><span class="sxs-lookup"><span data-stu-id="87549-131">Request</span></span>
<span data-ttu-id="87549-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87549-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="87549-133">応答</span><span class="sxs-lookup"><span data-stu-id="87549-133">Response</span></span>
<span data-ttu-id="87549-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87549-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->