# <a name="range-insert"></a><span data-ttu-id="3efe9-101">範囲: 挿入</span><span class="sxs-lookup"><span data-stu-id="3efe9-101">Range: insert</span></span>

<span data-ttu-id="3efe9-p101">この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="3efe9-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="3efe9-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3efe9-104">Permissions</span></span>
<span data-ttu-id="3efe9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3efe9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3efe9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3efe9-107">Permission type</span></span>      | <span data-ttu-id="3efe9-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3efe9-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3efe9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3efe9-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3efe9-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3efe9-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3efe9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3efe9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3efe9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3efe9-112">Not supported.</span></span>    |
|<span data-ttu-id="3efe9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3efe9-113">Application</span></span> | <span data-ttu-id="3efe9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3efe9-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3efe9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3efe9-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="3efe9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3efe9-116">Request headers</span></span>
| <span data-ttu-id="3efe9-117">名前</span><span class="sxs-lookup"><span data-stu-id="3efe9-117">Name</span></span>       | <span data-ttu-id="3efe9-118">説明</span><span class="sxs-lookup"><span data-stu-id="3efe9-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3efe9-119">承認</span><span class="sxs-lookup"><span data-stu-id="3efe9-119">Authorization</span></span>  | <span data-ttu-id="3efe9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3efe9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3efe9-122">ブック セッション ID</span><span class="sxs-lookup"><span data-stu-id="3efe9-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="3efe9-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3efe9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3efe9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3efe9-125">Request body</span></span>
<span data-ttu-id="3efe9-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3efe9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3efe9-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3efe9-127">Parameter</span></span>    | <span data-ttu-id="3efe9-128">型</span><span class="sxs-lookup"><span data-stu-id="3efe9-128">Type</span></span>   |<span data-ttu-id="3efe9-129">説明</span><span class="sxs-lookup"><span data-stu-id="3efe9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3efe9-130"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="3efe9-130">shift</span></span>|<span data-ttu-id="3efe9-131">文字列</span><span class="sxs-lookup"><span data-stu-id="3efe9-131">string</span></span>|<span data-ttu-id="3efe9-132">セルをシフトする方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="3efe9-132">. Specifies which way to shift the cells.</span></span>  <span data-ttu-id="3efe9-133">指定できる値は、`Down`、`Right` です。</span><span class="sxs-lookup"><span data-stu-id="3efe9-133">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="3efe9-134">応答</span><span class="sxs-lookup"><span data-stu-id="3efe9-134">Response</span></span>

<span data-ttu-id="3efe9-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3efe9-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3efe9-136">例</span><span class="sxs-lookup"><span data-stu-id="3efe9-136">Example</span></span>
<span data-ttu-id="3efe9-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3efe9-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3efe9-138">要求</span><span class="sxs-lookup"><span data-stu-id="3efe9-138">Request</span></span>
<span data-ttu-id="3efe9-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3efe9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="3efe9-140">応答</span><span class="sxs-lookup"><span data-stu-id="3efe9-140">Response</span></span>
<span data-ttu-id="3efe9-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3efe9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->