# <a name="range-intersection"></a><span data-ttu-id="8807f-101">範囲:Intersection</span><span class="sxs-lookup"><span data-stu-id="8807f-101">Range: Intersection</span></span>

<span data-ttu-id="8807f-102">指定した範囲の長方形の交差を表す範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8807f-102">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="8807f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8807f-103">Permissions</span></span>
<span data-ttu-id="8807f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8807f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8807f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8807f-106">Permission type</span></span>      | <span data-ttu-id="8807f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8807f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8807f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8807f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8807f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8807f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8807f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8807f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8807f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8807f-111">Not supported.</span></span>    |
|<span data-ttu-id="8807f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8807f-112">Application</span></span> | <span data-ttu-id="8807f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8807f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8807f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8807f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="8807f-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8807f-115">Request headers</span></span>
| <span data-ttu-id="8807f-116">名前</span><span class="sxs-lookup"><span data-stu-id="8807f-116">Name</span></span>       | <span data-ttu-id="8807f-117">説明</span><span class="sxs-lookup"><span data-stu-id="8807f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8807f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="8807f-118">Authorization</span></span>  | <span data-ttu-id="8807f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8807f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8807f-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="8807f-121">Request body</span></span>
<span data-ttu-id="8807f-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8807f-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8807f-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8807f-123">Parameter</span></span>    | <span data-ttu-id="8807f-124">型</span><span class="sxs-lookup"><span data-stu-id="8807f-124">Type</span></span>   |<span data-ttu-id="8807f-125">説明</span><span class="sxs-lookup"><span data-stu-id="8807f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8807f-126">anotherRange</span><span class="sxs-lookup"><span data-stu-id="8807f-126">anotherRange</span></span>|<span data-ttu-id="8807f-127">string</span><span class="sxs-lookup"><span data-stu-id="8807f-127">string</span></span>|<span data-ttu-id="8807f-128">範囲の交差を判断するために使用される、Range オブジェクトまたは Range アドレス。</span><span class="sxs-lookup"><span data-stu-id="8807f-128">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="8807f-129">応答</span><span class="sxs-lookup"><span data-stu-id="8807f-129">Response</span></span>

<span data-ttu-id="8807f-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8807f-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8807f-131">例</span><span class="sxs-lookup"><span data-stu-id="8807f-131">Example</span></span>
<span data-ttu-id="8807f-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8807f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8807f-133">要求</span><span class="sxs-lookup"><span data-stu-id="8807f-133">Request</span></span>
<span data-ttu-id="8807f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8807f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="8807f-135">応答</span><span class="sxs-lookup"><span data-stu-id="8807f-135">Response</span></span>
<span data-ttu-id="8807f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8807f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->