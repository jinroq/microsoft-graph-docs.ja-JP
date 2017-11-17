# <a name="range-offsetrange"></a><span data-ttu-id="b7649-101">範囲:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="b7649-101">Range: OffsetRange</span></span>

<span data-ttu-id="b7649-p101">指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="b7649-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7649-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7649-105">Permissions</span></span>
<span data-ttu-id="b7649-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7649-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b7649-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7649-108">Permission type</span></span>      | <span data-ttu-id="b7649-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7649-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7649-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7649-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7649-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7649-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7649-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7649-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7649-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7649-113">Not supported.</span></span>    |
|<span data-ttu-id="b7649-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7649-114">Application</span></span> | <span data-ttu-id="b7649-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7649-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7649-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7649-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="b7649-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7649-117">Request headers</span></span>
| <span data-ttu-id="b7649-118">名前</span><span class="sxs-lookup"><span data-stu-id="b7649-118">Name</span></span>       | <span data-ttu-id="b7649-119">説明</span><span class="sxs-lookup"><span data-stu-id="b7649-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7649-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7649-120">Authorization</span></span>  | <span data-ttu-id="b7649-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7649-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7649-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7649-123">Request body</span></span>
<span data-ttu-id="b7649-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7649-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7649-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7649-125">Parameter</span></span>    | <span data-ttu-id="b7649-126">型</span><span class="sxs-lookup"><span data-stu-id="b7649-126">Type</span></span>   |<span data-ttu-id="b7649-127">説明</span><span class="sxs-lookup"><span data-stu-id="b7649-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7649-128">rowOffset</span><span class="sxs-lookup"><span data-stu-id="b7649-128">rowOffset</span></span>|<span data-ttu-id="b7649-129">number</span><span class="sxs-lookup"><span data-stu-id="b7649-129">number</span></span>|<span data-ttu-id="b7649-p104">範囲をオフセットする行数 (正、負、または 0)。正の値は下方向へのオフセットです。また、負の値は上方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="b7649-p104">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="b7649-132">columnOffset</span><span class="sxs-lookup"><span data-stu-id="b7649-132">columnOffset</span></span>|<span data-ttu-id="b7649-133">number</span><span class="sxs-lookup"><span data-stu-id="b7649-133">number</span></span>|<span data-ttu-id="b7649-p105">範囲をオフセットする列数 (正、負、または 0)。正の値は右方向へのオフセットです。また、負の値は左方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="b7649-p105">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="b7649-136">応答</span><span class="sxs-lookup"><span data-stu-id="b7649-136">Response</span></span>

<span data-ttu-id="b7649-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7649-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7649-138">例</span><span class="sxs-lookup"><span data-stu-id="b7649-138">Example</span></span>
<span data-ttu-id="b7649-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b7649-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7649-140">要求</span><span class="sxs-lookup"><span data-stu-id="b7649-140">Request</span></span>
<span data-ttu-id="b7649-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7649-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="b7649-142">応答</span><span class="sxs-lookup"><span data-stu-id="b7649-142">Response</span></span>
<span data-ttu-id="b7649-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7649-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->