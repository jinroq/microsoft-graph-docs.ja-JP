# <a name="tablerowcollection-add"></a><span data-ttu-id="454af-101">TableRowCollection: add　</span><span class="sxs-lookup"><span data-stu-id="454af-101">TableRowCollection: add</span></span>

<span data-ttu-id="454af-102">新しい行をテーブルに追加します。</span><span class="sxs-lookup"><span data-stu-id="454af-102">Adds a new row to the table.</span></span>

## <a name="error-handling"></a><span data-ttu-id="454af-103">エラー処理</span><span class="sxs-lookup"><span data-stu-id="454af-103">Error Handling</span></span>

<span data-ttu-id="454af-104">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="454af-104">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="454af-105">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="454af-105">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="454af-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="454af-106">Permissions</span></span>
<span data-ttu-id="454af-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="454af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="454af-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="454af-109">Permission type</span></span>      | <span data-ttu-id="454af-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="454af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="454af-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="454af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="454af-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="454af-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="454af-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="454af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="454af-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="454af-114">Not supported.</span></span>    |
|<span data-ttu-id="454af-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="454af-115">Application</span></span> | <span data-ttu-id="454af-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="454af-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="454af-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="454af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="454af-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="454af-118">Request headers</span></span>
| <span data-ttu-id="454af-119">名前</span><span class="sxs-lookup"><span data-stu-id="454af-119">Name</span></span>       | <span data-ttu-id="454af-120">説明</span><span class="sxs-lookup"><span data-stu-id="454af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="454af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="454af-121">Authorization</span></span>  | <span data-ttu-id="454af-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="454af-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="454af-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="454af-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="454af-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="454af-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="454af-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="454af-127">Request body</span></span>
<span data-ttu-id="454af-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="454af-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="454af-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="454af-129">Parameter</span></span>    | <span data-ttu-id="454af-130">型</span><span class="sxs-lookup"><span data-stu-id="454af-130">Type</span></span>   |<span data-ttu-id="454af-131">説明</span><span class="sxs-lookup"><span data-stu-id="454af-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="454af-132">index</span><span class="sxs-lookup"><span data-stu-id="454af-132">index</span></span>|<span data-ttu-id="454af-133">number</span><span class="sxs-lookup"><span data-stu-id="454af-133">number</span></span>|<span data-ttu-id="454af-p105">省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="454af-p105">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="454af-139">values</span><span class="sxs-lookup"><span data-stu-id="454af-139">values</span></span>|<span data-ttu-id="454af-140">(boolean、string、または number)</span><span class="sxs-lookup"><span data-stu-id="454af-140">(boolean or string or number)</span></span>|<span data-ttu-id="454af-p106">省略可能。テーブルの行の書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="454af-p106">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="454af-143">応答</span><span class="sxs-lookup"><span data-stu-id="454af-143">Response</span></span>

<span data-ttu-id="454af-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="454af-144">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="454af-145">例</span><span class="sxs-lookup"><span data-stu-id="454af-145">Example</span></span>
<span data-ttu-id="454af-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="454af-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="454af-147">要求</span><span class="sxs-lookup"><span data-stu-id="454af-147">Request</span></span>
<span data-ttu-id="454af-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="454af-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="454af-149">応答</span><span class="sxs-lookup"><span data-stu-id="454af-149">Response</span></span>
<span data-ttu-id="454af-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="454af-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
