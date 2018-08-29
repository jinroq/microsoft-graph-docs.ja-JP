# <a name="create-tablerow"></a><span data-ttu-id="728cf-101">TableRow を作成する</span><span class="sxs-lookup"><span data-stu-id="728cf-101">Create TableRow</span></span>

<span data-ttu-id="728cf-102">テーブルの末尾に行を追加します。</span><span class="sxs-lookup"><span data-stu-id="728cf-102">Adds a row to the end of the table.</span></span> <span data-ttu-id="728cf-103">API がこの API を使用して複数の行データを受け入れることができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="728cf-103">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="728cf-104">一度に 1 行を追加すると、パフォーマンスが低下する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="728cf-104">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="728cf-105">推奨されるアプローチは、1 つの行の挿入を行うのではなく、1 回の呼び出しでまとめて行をバッチ処理することです。</span><span class="sxs-lookup"><span data-stu-id="728cf-105">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="728cf-106">最良の結果を得るには、収集アプリケーション側で挿入して、1 つの行を実行する行操作を追加します。</span><span class="sxs-lookup"><span data-stu-id="728cf-106">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="728cf-107">理想的な 1 つの API 呼び出しで使用する行の数を決定する行の番号を試してください。</span><span class="sxs-lookup"><span data-stu-id="728cf-107">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="728cf-108">エラー処理</span><span class="sxs-lookup"><span data-stu-id="728cf-108">Error Handling</span></span>

<span data-ttu-id="728cf-109">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="728cf-109">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="728cf-110">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="728cf-110">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="728cf-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="728cf-111">Permissions</span></span>
<span data-ttu-id="728cf-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="728cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="728cf-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="728cf-114">Permission type</span></span>      | <span data-ttu-id="728cf-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="728cf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="728cf-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="728cf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="728cf-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="728cf-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="728cf-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="728cf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="728cf-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="728cf-119">Not supported.</span></span>    |
|<span data-ttu-id="728cf-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="728cf-120">Application</span></span> | <span data-ttu-id="728cf-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="728cf-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="728cf-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="728cf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="728cf-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="728cf-123">Request headers</span></span>
| <span data-ttu-id="728cf-124">名前</span><span class="sxs-lookup"><span data-stu-id="728cf-124">Name</span></span>       | <span data-ttu-id="728cf-125">説明</span><span class="sxs-lookup"><span data-stu-id="728cf-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="728cf-126">承認</span><span class="sxs-lookup"><span data-stu-id="728cf-126">Authorization</span></span>  | <span data-ttu-id="728cf-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="728cf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="728cf-129">ブック セッション-Id</span><span class="sxs-lookup"><span data-stu-id="728cf-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="728cf-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="728cf-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="728cf-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="728cf-132">Request body</span></span>
<span data-ttu-id="728cf-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="728cf-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="728cf-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="728cf-134">Parameter</span></span>    | <span data-ttu-id="728cf-135">型</span><span class="sxs-lookup"><span data-stu-id="728cf-135">Type</span></span>   |<span data-ttu-id="728cf-136">説明</span><span class="sxs-lookup"><span data-stu-id="728cf-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="728cf-137">インデックス</span><span class="sxs-lookup"><span data-stu-id="728cf-137">index</span></span>|<span data-ttu-id="728cf-138">number</span><span class="sxs-lookup"><span data-stu-id="728cf-138">number</span></span>|<span data-ttu-id="728cf-p106">省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="728cf-p106">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="728cf-144">values</span><span class="sxs-lookup"><span data-stu-id="728cf-144">values</span></span>|<span data-ttu-id="728cf-145">Json</span><span class="sxs-lookup"><span data-stu-id="728cf-145">Json</span></span>|<span data-ttu-id="728cf-146">(ブール値または文字列または数値) のテーブルの行の書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="728cf-146">A 2-dimensional array of unformatted values of the table rows (boolean or string or number).</span></span>|

## <a name="response"></a><span data-ttu-id="728cf-147">応答</span><span class="sxs-lookup"><span data-stu-id="728cf-147">Response</span></span>

<span data-ttu-id="728cf-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="728cf-148">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="728cf-149">例</span><span class="sxs-lookup"><span data-stu-id="728cf-149">Example</span></span>
<span data-ttu-id="728cf-150">この例では、テーブルの末尾に 2 行のデータが挿入されます。</span><span class="sxs-lookup"><span data-stu-id="728cf-150">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="728cf-151">要求</span><span class="sxs-lookup"><span data-stu-id="728cf-151">Request</span></span>
<span data-ttu-id="728cf-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="728cf-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
##### <a name="response"></a><span data-ttu-id="728cf-153">応答</span><span class="sxs-lookup"><span data-stu-id="728cf-153">Response</span></span>
<span data-ttu-id="728cf-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="728cf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not.",
    "Warning: /api-reference/v1.0/api/table_post_rows.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)"
  ],
  "tocPath": ""
}-->
