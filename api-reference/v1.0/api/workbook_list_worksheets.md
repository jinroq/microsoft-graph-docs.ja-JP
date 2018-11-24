# <a name="list-worksheets"></a><span data-ttu-id="e7435-101">ワークシートを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e7435-101">List worksheets</span></span>

<span data-ttu-id="e7435-102">ワークシート オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e7435-102">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7435-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7435-103">Permissions</span></span>
<span data-ttu-id="e7435-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7435-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7435-106">Permission type</span></span>      | <span data-ttu-id="e7435-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7435-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7435-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7435-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e7435-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7435-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7435-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7435-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7435-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7435-111">Not supported.</span></span>    |
|<span data-ttu-id="e7435-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7435-112">Application</span></span> | <span data-ttu-id="e7435-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7435-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7435-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7435-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7435-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7435-115">Optional query parameters</span></span>
<span data-ttu-id="e7435-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e7435-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7435-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7435-117">Request headers</span></span>
| <span data-ttu-id="e7435-118">名前</span><span class="sxs-lookup"><span data-stu-id="e7435-118">Name</span></span>      |<span data-ttu-id="e7435-119">説明</span><span class="sxs-lookup"><span data-stu-id="e7435-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e7435-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7435-120">Authorization</span></span>  | <span data-ttu-id="e7435-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7435-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7435-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7435-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7435-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e7435-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7435-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7435-126">Request body</span></span>
<span data-ttu-id="e7435-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7435-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7435-128">応答</span><span class="sxs-lookup"><span data-stu-id="e7435-128">Response</span></span>

<span data-ttu-id="e7435-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookWorksheet](../resources/worksheet.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e7435-129">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7435-130">例</span><span class="sxs-lookup"><span data-stu-id="e7435-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7435-131">要求</span><span class="sxs-lookup"><span data-stu-id="e7435-131">Request</span></span>
<span data-ttu-id="e7435-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7435-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="e7435-133">応答</span><span class="sxs-lookup"><span data-stu-id="e7435-133">Response</span></span>
<span data-ttu-id="e7435-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7435-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->