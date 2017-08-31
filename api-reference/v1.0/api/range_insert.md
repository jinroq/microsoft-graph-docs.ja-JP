# <a name="range-insert"></a><span data-ttu-id="fdfe0-101">範囲: 挿入</span><span class="sxs-lookup"><span data-stu-id="fdfe0-101">Range: insert</span></span>

<span data-ttu-id="fdfe0-p101">この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdfe0-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fdfe0-104">Permissions</span></span>
<span data-ttu-id="fdfe0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdfe0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fdfe0-107">Permission type</span></span>      | <span data-ttu-id="fdfe0-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fdfe0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdfe0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfe0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fdfe0-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdfe0-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fdfe0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fdfe0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdfe0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-112">Not supported.</span></span>    |
|<span data-ttu-id="fdfe0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fdfe0-113">Application</span></span> | <span data-ttu-id="fdfe0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdfe0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fdfe0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(<address>)/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="fdfe0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fdfe0-116">Request headers</span></span>
| <span data-ttu-id="fdfe0-117">名前</span><span class="sxs-lookup"><span data-stu-id="fdfe0-117">Name</span></span>       | <span data-ttu-id="fdfe0-118">説明</span><span class="sxs-lookup"><span data-stu-id="fdfe0-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fdfe0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdfe0-119">Authorization</span></span>  | <span data-ttu-id="fdfe0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdfe0-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="fdfe0-122">Request body</span></span>
<span data-ttu-id="fdfe0-123">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fdfe0-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fdfe0-124">Parameter</span></span>    | <span data-ttu-id="fdfe0-125">型</span><span class="sxs-lookup"><span data-stu-id="fdfe0-125">Type</span></span>   |<span data-ttu-id="fdfe0-126">説明</span><span class="sxs-lookup"><span data-stu-id="fdfe0-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdfe0-127"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="fdfe0-127">shift</span></span>|<span data-ttu-id="fdfe0-128">string</span><span class="sxs-lookup"><span data-stu-id="fdfe0-128">string</span></span>|<span data-ttu-id="fdfe0-p104">セルをシフトする方向を指定します。可能な値は、`Down`、`Right` です。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-p104">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="fdfe0-131">応答</span><span class="sxs-lookup"><span data-stu-id="fdfe0-131">Response</span></span>

<span data-ttu-id="fdfe0-132">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-132">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdfe0-133">例</span><span class="sxs-lookup"><span data-stu-id="fdfe0-133">Example</span></span>
<span data-ttu-id="fdfe0-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fdfe0-135">要求</span><span class="sxs-lookup"><span data-stu-id="fdfe0-135">Request</span></span>
<span data-ttu-id="fdfe0-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="fdfe0-137">応答</span><span class="sxs-lookup"><span data-stu-id="fdfe0-137">Response</span></span>
<span data-ttu-id="fdfe0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fdfe0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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