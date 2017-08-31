# <a name="chartcollection-itemat"></a><span data-ttu-id="83c4f-101">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="83c4f-101">ChartCollection: ItemAt</span></span>

<span data-ttu-id="83c4f-102">コレクション内での位置を基にグラフを取得します。</span><span class="sxs-lookup"><span data-stu-id="83c4f-102">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="83c4f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83c4f-103">Permissions</span></span>
<span data-ttu-id="83c4f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83c4f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83c4f-106">Permission type</span></span>      | <span data-ttu-id="83c4f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83c4f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83c4f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83c4f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="83c4f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83c4f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83c4f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83c4f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c4f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83c4f-111">Not supported.</span></span>    |
|<span data-ttu-id="83c4f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83c4f-112">Application</span></span> | <span data-ttu-id="83c4f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83c4f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83c4f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83c4f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="83c4f-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83c4f-115">Request headers</span></span>
| <span data-ttu-id="83c4f-116">名前</span><span class="sxs-lookup"><span data-stu-id="83c4f-116">Name</span></span>       | <span data-ttu-id="83c4f-117">説明</span><span class="sxs-lookup"><span data-stu-id="83c4f-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83c4f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="83c4f-118">Authorization</span></span>  | <span data-ttu-id="83c4f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83c4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83c4f-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="83c4f-121">Request body</span></span>
<span data-ttu-id="83c4f-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="83c4f-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83c4f-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="83c4f-123">Parameter</span></span>    | <span data-ttu-id="83c4f-124">型</span><span class="sxs-lookup"><span data-stu-id="83c4f-124">Type</span></span>   |<span data-ttu-id="83c4f-125">説明</span><span class="sxs-lookup"><span data-stu-id="83c4f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83c4f-126">index</span><span class="sxs-lookup"><span data-stu-id="83c4f-126">index</span></span>|<span data-ttu-id="83c4f-127">number</span><span class="sxs-lookup"><span data-stu-id="83c4f-127">number</span></span>|<span data-ttu-id="83c4f-p103">取得するオブジェクトのインデックス値。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="83c4f-p103">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="83c4f-130">応答</span><span class="sxs-lookup"><span data-stu-id="83c4f-130">Response</span></span>

<span data-ttu-id="83c4f-131">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83c4f-131">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83c4f-132">例</span><span class="sxs-lookup"><span data-stu-id="83c4f-132">Example</span></span>
<span data-ttu-id="83c4f-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="83c4f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="83c4f-134">要求</span><span class="sxs-lookup"><span data-stu-id="83c4f-134">Request</span></span>
<span data-ttu-id="83c4f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83c4f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="83c4f-136">応答</span><span class="sxs-lookup"><span data-stu-id="83c4f-136">Response</span></span>
<span data-ttu-id="83c4f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83c4f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->