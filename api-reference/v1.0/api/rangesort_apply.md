# <a name="rangesort-apply"></a><span data-ttu-id="155d5-101">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="155d5-101">RangeSort: apply</span></span>

<span data-ttu-id="155d5-102">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="155d5-102">Perform a sort operation.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="155d5-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="155d5-103">Prerequisites</span></span>
<span data-ttu-id="155d5-104">この API を実行するために必要な**スコープ**は、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="155d5-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="155d5-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="155d5-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="155d5-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="155d5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="155d5-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="155d5-107">Request headers</span></span>
| <span data-ttu-id="155d5-108">名前</span><span class="sxs-lookup"><span data-stu-id="155d5-108">Name</span></span>       | <span data-ttu-id="155d5-109">説明</span><span class="sxs-lookup"><span data-stu-id="155d5-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="155d5-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="155d5-110">Authorization</span></span>  | <span data-ttu-id="155d5-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="155d5-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="155d5-113">要求本文</span><span class="sxs-lookup"><span data-stu-id="155d5-113">Request body</span></span>
<span data-ttu-id="155d5-114">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="155d5-114">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="155d5-115">パラメーター</span><span class="sxs-lookup"><span data-stu-id="155d5-115">Parameter</span></span>    | <span data-ttu-id="155d5-116">型</span><span class="sxs-lookup"><span data-stu-id="155d5-116">Type</span></span>   |<span data-ttu-id="155d5-117">説明</span><span class="sxs-lookup"><span data-stu-id="155d5-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="155d5-118">fields</span><span class="sxs-lookup"><span data-stu-id="155d5-118">fields</span></span>|<span data-ttu-id="155d5-119">SortField</span><span class="sxs-lookup"><span data-stu-id="155d5-119">SortField</span></span>|<span data-ttu-id="155d5-120">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="155d5-120">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="155d5-121">matchCase</span><span class="sxs-lookup"><span data-stu-id="155d5-121">matchCase</span></span>|<span data-ttu-id="155d5-122">boolean</span><span class="sxs-lookup"><span data-stu-id="155d5-122">boolean</span></span>|<span data-ttu-id="155d5-p102">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="155d5-p102">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="155d5-125">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="155d5-125">hasHeaders</span></span>|<span data-ttu-id="155d5-126">boolean</span><span class="sxs-lookup"><span data-stu-id="155d5-126">boolean</span></span>|<span data-ttu-id="155d5-p103">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="155d5-p103">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="155d5-129">orientation</span><span class="sxs-lookup"><span data-stu-id="155d5-129">orientation</span></span>|<span data-ttu-id="155d5-130">string</span><span class="sxs-lookup"><span data-stu-id="155d5-130">string</span></span>|<span data-ttu-id="155d5-p104">省略可能。操作が行と列のどちらの並べ替えかを示します。可能な値は、`Rows`、`Columns` です。</span><span class="sxs-lookup"><span data-stu-id="155d5-p104">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="155d5-134">method</span><span class="sxs-lookup"><span data-stu-id="155d5-134">method</span></span>|<span data-ttu-id="155d5-135">string</span><span class="sxs-lookup"><span data-stu-id="155d5-135">string</span></span>|<span data-ttu-id="155d5-p105">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="155d5-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="155d5-139">応答</span><span class="sxs-lookup"><span data-stu-id="155d5-139">Response</span></span>

<span data-ttu-id="155d5-p106">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="155d5-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="155d5-142">例</span><span class="sxs-lookup"><span data-stu-id="155d5-142">Example</span></span>
<span data-ttu-id="155d5-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="155d5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="155d5-144">要求</span><span class="sxs-lookup"><span data-stu-id="155d5-144">Request</span></span>
<span data-ttu-id="155d5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="155d5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="155d5-146">応答</span><span class="sxs-lookup"><span data-stu-id="155d5-146">Response</span></span>
<span data-ttu-id="155d5-147">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="155d5-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->