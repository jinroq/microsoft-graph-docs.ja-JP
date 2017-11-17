# <a name="tablerowcollection-add"></a><span data-ttu-id="23bb0-101">TableRowCollection: add　</span><span class="sxs-lookup"><span data-stu-id="23bb0-101">TableRowCollection: add</span></span>

<span data-ttu-id="23bb0-102">新しい行をテーブルに追加します。</span><span class="sxs-lookup"><span data-stu-id="23bb0-102">Adds a new row to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="23bb0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="23bb0-103">Permissions</span></span>
<span data-ttu-id="23bb0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23bb0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23bb0-106">Permission type</span></span>      | <span data-ttu-id="23bb0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="23bb0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23bb0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23bb0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="23bb0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23bb0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23bb0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23bb0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23bb0-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23bb0-111">Not supported.</span></span>    |
|<span data-ttu-id="23bb0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23bb0-112">Application</span></span> | <span data-ttu-id="23bb0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23bb0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23bb0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23bb0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="23bb0-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23bb0-115">Request headers</span></span>
| <span data-ttu-id="23bb0-116">名前</span><span class="sxs-lookup"><span data-stu-id="23bb0-116">Name</span></span>       | <span data-ttu-id="23bb0-117">説明</span><span class="sxs-lookup"><span data-stu-id="23bb0-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23bb0-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="23bb0-118">Authorization</span></span>  | <span data-ttu-id="23bb0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="23bb0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23bb0-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="23bb0-121">Request body</span></span>
<span data-ttu-id="23bb0-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="23bb0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23bb0-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="23bb0-123">Parameter</span></span>    | <span data-ttu-id="23bb0-124">型</span><span class="sxs-lookup"><span data-stu-id="23bb0-124">Type</span></span>   |<span data-ttu-id="23bb0-125">説明</span><span class="sxs-lookup"><span data-stu-id="23bb0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23bb0-126">index</span><span class="sxs-lookup"><span data-stu-id="23bb0-126">index</span></span>|<span data-ttu-id="23bb0-127">number</span><span class="sxs-lookup"><span data-stu-id="23bb0-127">number</span></span>|<span data-ttu-id="23bb0-p103">省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="23bb0-p103">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="23bb0-133">values</span><span class="sxs-lookup"><span data-stu-id="23bb0-133">values</span></span>|<span data-ttu-id="23bb0-134">(boolean、string、または number)</span><span class="sxs-lookup"><span data-stu-id="23bb0-134">(boolean or string or number)</span></span>|<span data-ttu-id="23bb0-p104">省略可能。テーブルの行の書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="23bb0-p104">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="23bb0-137">応答</span><span class="sxs-lookup"><span data-stu-id="23bb0-137">Response</span></span>

<span data-ttu-id="23bb0-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23bb0-138">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23bb0-139">例</span><span class="sxs-lookup"><span data-stu-id="23bb0-139">Example</span></span>
<span data-ttu-id="23bb0-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="23bb0-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23bb0-141">要求</span><span class="sxs-lookup"><span data-stu-id="23bb0-141">Request</span></span>
<span data-ttu-id="23bb0-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23bb0-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="23bb0-143">応答</span><span class="sxs-lookup"><span data-stu-id="23bb0-143">Response</span></span>
<span data-ttu-id="23bb0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23bb0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
