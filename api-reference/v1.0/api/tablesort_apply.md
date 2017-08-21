# <a name="tablesort-apply"></a><span data-ttu-id="88174-101">TableSort: apply　</span><span class="sxs-lookup"><span data-stu-id="88174-101">TableSort: apply</span></span>

<span data-ttu-id="88174-102">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="88174-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88174-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="88174-103">Prerequisites</span></span>
<span data-ttu-id="88174-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="88174-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="88174-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88174-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="88174-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88174-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="88174-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88174-107">Request headers</span></span>
| <span data-ttu-id="88174-108">名前</span><span class="sxs-lookup"><span data-stu-id="88174-108">Name</span></span>       | <span data-ttu-id="88174-109">説明</span><span class="sxs-lookup"><span data-stu-id="88174-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88174-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="88174-110">Authorization</span></span>  | <span data-ttu-id="88174-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88174-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="88174-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="88174-113">Request body</span></span>
<span data-ttu-id="88174-114">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="88174-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="88174-115">パラメーター</span><span class="sxs-lookup"><span data-stu-id="88174-115">Parameter</span></span>    | <span data-ttu-id="88174-116">型</span><span class="sxs-lookup"><span data-stu-id="88174-116">Type</span></span>   |<span data-ttu-id="88174-117">説明</span><span class="sxs-lookup"><span data-stu-id="88174-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88174-118">fields</span><span class="sxs-lookup"><span data-stu-id="88174-118">fields</span></span>|<span data-ttu-id="88174-119">SortField</span><span class="sxs-lookup"><span data-stu-id="88174-119">SortField</span></span>|<span data-ttu-id="88174-120">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="88174-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="88174-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="88174-121">matchCase</span></span>|<span data-ttu-id="88174-122">boolean</span><span class="sxs-lookup"><span data-stu-id="88174-122">boolean</span></span>|<span data-ttu-id="88174-p102">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="88174-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="88174-125">method</span><span class="sxs-lookup"><span data-stu-id="88174-125">method</span></span>|<span data-ttu-id="88174-126">string</span><span class="sxs-lookup"><span data-stu-id="88174-126">string</span></span>|<span data-ttu-id="88174-p103">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="88174-p103">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="88174-130">応答</span><span class="sxs-lookup"><span data-stu-id="88174-130">Response</span></span>

<span data-ttu-id="88174-p104">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="88174-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88174-133">例</span><span class="sxs-lookup"><span data-stu-id="88174-133">Example</span></span>
<span data-ttu-id="88174-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="88174-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88174-135">要求</span><span class="sxs-lookup"><span data-stu-id="88174-135">Request</span></span>
<span data-ttu-id="88174-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88174-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="88174-137">応答</span><span class="sxs-lookup"><span data-stu-id="88174-137">Response</span></span>
<span data-ttu-id="88174-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="88174-138">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->