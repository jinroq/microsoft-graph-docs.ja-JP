# <a name="range-row"></a><span data-ttu-id="3f2e2-101">範囲:Row</span><span class="sxs-lookup"><span data-stu-id="3f2e2-101">Range: Row</span></span>

<span data-ttu-id="3f2e2-102">範囲に含まれている行を 1 つ取得します。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-102">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f2e2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f2e2-103">Permissions</span></span>
<span data-ttu-id="3f2e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3f2e2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f2e2-106">Permission type</span></span>      | <span data-ttu-id="3f2e2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f2e2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f2e2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f2e2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3f2e2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3f2e2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3f2e2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f2e2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f2e2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-111">Not supported.</span></span>    |
|<span data-ttu-id="3f2e2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f2e2-112">Application</span></span> | <span data-ttu-id="3f2e2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f2e2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f2e2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="3f2e2-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f2e2-115">Request headers</span></span>
| <span data-ttu-id="3f2e2-116">名前</span><span class="sxs-lookup"><span data-stu-id="3f2e2-116">Name</span></span>       | <span data-ttu-id="3f2e2-117">説明</span><span class="sxs-lookup"><span data-stu-id="3f2e2-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3f2e2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f2e2-118">Authorization</span></span>  | <span data-ttu-id="3f2e2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3f2e2-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3f2e2-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3f2e2-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f2e2-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f2e2-124">Request body</span></span>
<span data-ttu-id="3f2e2-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f2e2-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3f2e2-126">Parameter</span></span>    | <span data-ttu-id="3f2e2-127">Type</span><span class="sxs-lookup"><span data-stu-id="3f2e2-127">Type</span></span>   |<span data-ttu-id="3f2e2-128">説明</span><span class="sxs-lookup"><span data-stu-id="3f2e2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f2e2-129">row</span><span class="sxs-lookup"><span data-stu-id="3f2e2-129">row</span></span>|<span data-ttu-id="3f2e2-130">number</span><span class="sxs-lookup"><span data-stu-id="3f2e2-130">number</span></span>|<span data-ttu-id="3f2e2-p104">取得する範囲の行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="3f2e2-133">応答</span><span class="sxs-lookup"><span data-stu-id="3f2e2-133">Response</span></span>

<span data-ttu-id="3f2e2-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f2e2-135">例</span><span class="sxs-lookup"><span data-stu-id="3f2e2-135">Example</span></span>
<span data-ttu-id="3f2e2-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3f2e2-137">要求</span><span class="sxs-lookup"><span data-stu-id="3f2e2-137">Request</span></span>
<span data-ttu-id="3f2e2-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="3f2e2-139">応答</span><span class="sxs-lookup"><span data-stu-id="3f2e2-139">Response</span></span>
<span data-ttu-id="3f2e2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f2e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->