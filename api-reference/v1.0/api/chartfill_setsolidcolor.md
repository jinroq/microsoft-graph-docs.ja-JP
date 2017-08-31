# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="c8213-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="c8213-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="c8213-102">グラフ要素の塗りつぶしの書式設定を均一な色に設定します。</span><span class="sxs-lookup"><span data-stu-id="c8213-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8213-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8213-103">Permissions</span></span>
<span data-ttu-id="c8213-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c8213-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8213-106">Permission type</span></span>      | <span data-ttu-id="c8213-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8213-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8213-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8213-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c8213-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8213-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8213-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8213-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8213-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8213-111">Not supported.</span></span>    |
|<span data-ttu-id="c8213-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8213-112">Application</span></span> | <span data-ttu-id="c8213-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8213-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8213-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8213-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="c8213-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8213-115">Request headers</span></span>
| <span data-ttu-id="c8213-116">名前</span><span class="sxs-lookup"><span data-stu-id="c8213-116">Name</span></span>       | <span data-ttu-id="c8213-117">説明</span><span class="sxs-lookup"><span data-stu-id="c8213-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8213-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8213-118">Authorization</span></span>  | <span data-ttu-id="c8213-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8213-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8213-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8213-121">Request body</span></span>
<span data-ttu-id="c8213-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8213-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8213-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8213-123">Parameter</span></span>    | <span data-ttu-id="c8213-124">型</span><span class="sxs-lookup"><span data-stu-id="c8213-124">Type</span></span>   |<span data-ttu-id="c8213-125">説明</span><span class="sxs-lookup"><span data-stu-id="c8213-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8213-126">color</span><span class="sxs-lookup"><span data-stu-id="c8213-126">color</span></span>|<span data-ttu-id="c8213-127">string</span><span class="sxs-lookup"><span data-stu-id="c8213-127">string</span></span>|<span data-ttu-id="c8213-128">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="c8213-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="c8213-129">応答</span><span class="sxs-lookup"><span data-stu-id="c8213-129">Response</span></span>

<span data-ttu-id="c8213-p103">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c8213-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8213-132">例</span><span class="sxs-lookup"><span data-stu-id="c8213-132">Example</span></span>
<span data-ttu-id="c8213-133">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c8213-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8213-134">要求</span><span class="sxs-lookup"><span data-stu-id="c8213-134">Request</span></span>
<span data-ttu-id="c8213-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8213-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="c8213-136">応答</span><span class="sxs-lookup"><span data-stu-id="c8213-136">Response</span></span>
<span data-ttu-id="c8213-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c8213-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->