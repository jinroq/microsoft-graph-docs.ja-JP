# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="b91a1-101">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="b91a1-101">ChartFill: setSolidColor</span></span>

<span data-ttu-id="b91a1-102">グラフ要素の塗りつぶしの書式設定を均一な色に設定します。</span><span class="sxs-lookup"><span data-stu-id="b91a1-102">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="b91a1-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b91a1-103">Permissions</span></span>
<span data-ttu-id="b91a1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b91a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b91a1-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b91a1-106">Permission type</span></span>      | <span data-ttu-id="b91a1-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b91a1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b91a1-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b91a1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b91a1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b91a1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b91a1-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b91a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b91a1-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b91a1-111">Not supported.</span></span>    |
|<span data-ttu-id="b91a1-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b91a1-112">Application</span></span> | <span data-ttu-id="b91a1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b91a1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b91a1-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b91a1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="b91a1-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b91a1-115">Request headers</span></span>
| <span data-ttu-id="b91a1-116">名前</span><span class="sxs-lookup"><span data-stu-id="b91a1-116">Name</span></span>       | <span data-ttu-id="b91a1-117">説明</span><span class="sxs-lookup"><span data-stu-id="b91a1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b91a1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="b91a1-118">Authorization</span></span>  | <span data-ttu-id="b91a1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b91a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b91a1-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b91a1-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="b91a1-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b91a1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b91a1-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b91a1-124">Request body</span></span>
<span data-ttu-id="b91a1-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b91a1-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b91a1-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b91a1-126">Parameter</span></span>    | <span data-ttu-id="b91a1-127">Type</span><span class="sxs-lookup"><span data-stu-id="b91a1-127">Type</span></span>   |<span data-ttu-id="b91a1-128">説明</span><span class="sxs-lookup"><span data-stu-id="b91a1-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b91a1-129">color</span><span class="sxs-lookup"><span data-stu-id="b91a1-129">color</span></span>|<span data-ttu-id="b91a1-130">string</span><span class="sxs-lookup"><span data-stu-id="b91a1-130">string</span></span>|<span data-ttu-id="b91a1-131">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="b91a1-131">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="b91a1-132">応答</span><span class="sxs-lookup"><span data-stu-id="b91a1-132">Response</span></span>

<span data-ttu-id="b91a1-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b91a1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b91a1-135">例</span><span class="sxs-lookup"><span data-stu-id="b91a1-135">Example</span></span>
<span data-ttu-id="b91a1-136">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b91a1-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b91a1-137">要求</span><span class="sxs-lookup"><span data-stu-id="b91a1-137">Request</span></span>
<span data-ttu-id="b91a1-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b91a1-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b91a1-139">応答</span><span class="sxs-lookup"><span data-stu-id="b91a1-139">Response</span></span>
<span data-ttu-id="b91a1-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b91a1-140">Here is an example of the response.</span></span> 
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