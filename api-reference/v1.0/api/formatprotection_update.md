# <a name="update-formatprotection"></a><span data-ttu-id="9d533-101">FormatProtection オブジェクトの更新</span><span class="sxs-lookup"><span data-stu-id="9d533-101">Update formatprotection</span></span>

<span data-ttu-id="9d533-102">formatprotection オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d533-102">Update the properties of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d533-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d533-103">Prerequisites</span></span>
<span data-ttu-id="9d533-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9d533-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="9d533-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d533-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="9d533-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d533-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="9d533-107">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d533-107">Optional request headers</span></span>
| <span data-ttu-id="9d533-108">名前</span><span class="sxs-lookup"><span data-stu-id="9d533-108">Name</span></span>       | <span data-ttu-id="9d533-109">説明</span><span class="sxs-lookup"><span data-stu-id="9d533-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d533-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d533-110">Authorization</span></span>  | <span data-ttu-id="9d533-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d533-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d533-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d533-113">Request body</span></span>
<span data-ttu-id="9d533-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9d533-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d533-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d533-117">Property</span></span>     | <span data-ttu-id="9d533-118">型</span><span class="sxs-lookup"><span data-stu-id="9d533-118">Type</span></span>   |<span data-ttu-id="9d533-119">説明</span><span class="sxs-lookup"><span data-stu-id="9d533-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d533-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="9d533-120">formulaHidden</span></span>|<span data-ttu-id="9d533-121">boolean</span><span class="sxs-lookup"><span data-stu-id="9d533-121">boolean</span></span>|<span data-ttu-id="9d533-p103">Excel が範囲内のセルの数式を非表示にするかどうかを示します。null 値は、範囲全体に一様な数式非表示設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="9d533-p103">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="9d533-124">locked</span><span class="sxs-lookup"><span data-stu-id="9d533-124">locked</span></span>|<span data-ttu-id="9d533-125">boolean</span><span class="sxs-lookup"><span data-stu-id="9d533-125">boolean</span></span>|<span data-ttu-id="9d533-p104">Excel がオブジェクト内のセルをロックするかどうかを示します。null 値は、範囲全体に一様なロック設定がないことを表します。</span><span class="sxs-lookup"><span data-stu-id="9d533-p104">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="9d533-128">応答</span><span class="sxs-lookup"><span data-stu-id="9d533-128">Response</span></span>

<span data-ttu-id="9d533-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [FormatProtection](../resources/formatprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d533-129">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d533-130">例</span><span class="sxs-lookup"><span data-stu-id="9d533-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d533-131">要求</span><span class="sxs-lookup"><span data-stu-id="9d533-131">Request</span></span>
<span data-ttu-id="9d533-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d533-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="9d533-133">応答</span><span class="sxs-lookup"><span data-stu-id="9d533-133">Response</span></span>
<span data-ttu-id="9d533-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d533-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->