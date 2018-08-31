# <a name="range-usedrange"></a><span data-ttu-id="ebd9a-101">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="ebd9a-101">Range: UsedRange</span></span>

<span data-ttu-id="ebd9a-102">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-102">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebd9a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ebd9a-103">Permissions</span></span>
<span data-ttu-id="ebd9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebd9a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebd9a-106">Permission type</span></span>      | <span data-ttu-id="ebd9a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebd9a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebd9a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebd9a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ebd9a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebd9a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebd9a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebd9a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebd9a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-111">Not supported.</span></span>    |
|<span data-ttu-id="ebd9a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebd9a-112">Application</span></span> | <span data-ttu-id="ebd9a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebd9a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebd9a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="ebd9a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebd9a-115">Request headers</span></span>
| <span data-ttu-id="ebd9a-116">名前</span><span class="sxs-lookup"><span data-stu-id="ebd9a-116">Name</span></span>       | <span data-ttu-id="ebd9a-117">説明</span><span class="sxs-lookup"><span data-stu-id="ebd9a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebd9a-118">承認</span><span class="sxs-lookup"><span data-stu-id="ebd9a-118">Authorization</span></span>  | <span data-ttu-id="ebd9a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebd9a-121">ブック セッション ID</span><span class="sxs-lookup"><span data-stu-id="ebd9a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebd9a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="ebd9a-124">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="ebd9a-124">Path parameters</span></span>
| <span data-ttu-id="ebd9a-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ebd9a-125">Parameter</span></span>    | <span data-ttu-id="ebd9a-126">型</span><span class="sxs-lookup"><span data-stu-id="ebd9a-126">Type</span></span>   |<span data-ttu-id="ebd9a-127">説明</span><span class="sxs-lookup"><span data-stu-id="ebd9a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebd9a-128">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="ebd9a-128">valuesOnly</span></span>|<span data-ttu-id="ebd9a-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="ebd9a-129">boolean</span></span>|<span data-ttu-id="ebd9a-p104">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="ebd9a-132">応答</span><span class="sxs-lookup"><span data-stu-id="ebd9a-132">Response</span></span>

<span data-ttu-id="ebd9a-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-133">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebd9a-134">例</span><span class="sxs-lookup"><span data-stu-id="ebd9a-134">Example</span></span>
<span data-ttu-id="ebd9a-135">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebd9a-136">要求</span><span class="sxs-lookup"><span data-stu-id="ebd9a-136">Request</span></span>
<span data-ttu-id="ebd9a-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-137">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="ebd9a-138">応答</span><span class="sxs-lookup"><span data-stu-id="ebd9a-138">Response</span></span>
<span data-ttu-id="ebd9a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="ebd9a-142">以下は、オプション `valuesOnly` のパラメーターを指定する例です。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-142">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="ebd9a-143">要求</span><span class="sxs-lookup"><span data-stu-id="ebd9a-143">Request</span></span>
<span data-ttu-id="ebd9a-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebd9a-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="ebd9a-145">応答</span><span class="sxs-lookup"><span data-stu-id="ebd9a-145">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->