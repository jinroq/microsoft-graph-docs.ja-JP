# <a name="rangesort-apply"></a><span data-ttu-id="774d2-101">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="774d2-101">RangeSort: apply</span></span>

<span data-ttu-id="774d2-102">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="774d2-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="774d2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="774d2-103">Permissions</span></span>
<span data-ttu-id="774d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="774d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="774d2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="774d2-106">Permission type</span></span>      | <span data-ttu-id="774d2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="774d2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="774d2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="774d2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="774d2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="774d2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="774d2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="774d2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="774d2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="774d2-111">Not supported.</span></span>    |
|<span data-ttu-id="774d2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="774d2-112">Application</span></span> | <span data-ttu-id="774d2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="774d2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="774d2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="774d2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(<address>)/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="774d2-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="774d2-115">Request headers</span></span>
| <span data-ttu-id="774d2-116">名前</span><span class="sxs-lookup"><span data-stu-id="774d2-116">Name</span></span>       | <span data-ttu-id="774d2-117">説明</span><span class="sxs-lookup"><span data-stu-id="774d2-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="774d2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="774d2-118">Authorization</span></span>  | <span data-ttu-id="774d2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="774d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="774d2-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="774d2-121">Request body</span></span>
<span data-ttu-id="774d2-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="774d2-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="774d2-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="774d2-123">Parameter</span></span>    | <span data-ttu-id="774d2-124">型</span><span class="sxs-lookup"><span data-stu-id="774d2-124">Type</span></span>   |<span data-ttu-id="774d2-125">説明</span><span class="sxs-lookup"><span data-stu-id="774d2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="774d2-126">fields</span><span class="sxs-lookup"><span data-stu-id="774d2-126">fields</span></span>|<span data-ttu-id="774d2-127">SortField</span><span class="sxs-lookup"><span data-stu-id="774d2-127">SortField</span></span>|<span data-ttu-id="774d2-128">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="774d2-128">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="774d2-129">matchCase</span><span class="sxs-lookup"><span data-stu-id="774d2-129">matchCase</span></span>|<span data-ttu-id="774d2-130">boolean</span><span class="sxs-lookup"><span data-stu-id="774d2-130">boolean</span></span>|<span data-ttu-id="774d2-p103">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="774d2-p103">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="774d2-133">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="774d2-133">hasHeaders</span></span>|<span data-ttu-id="774d2-134">boolean</span><span class="sxs-lookup"><span data-stu-id="774d2-134">boolean</span></span>|<span data-ttu-id="774d2-p104">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="774d2-p104">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="774d2-137">orientation</span><span class="sxs-lookup"><span data-stu-id="774d2-137">orientation</span></span>|<span data-ttu-id="774d2-138">string</span><span class="sxs-lookup"><span data-stu-id="774d2-138">string</span></span>|<span data-ttu-id="774d2-p105">省略可能。操作が行と列のどちらの並べ替えかを示します。可能な値は、`Rows`、`Columns` です。</span><span class="sxs-lookup"><span data-stu-id="774d2-p105">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="774d2-142">method</span><span class="sxs-lookup"><span data-stu-id="774d2-142">method</span></span>|<span data-ttu-id="774d2-143">string</span><span class="sxs-lookup"><span data-stu-id="774d2-143">string</span></span>|<span data-ttu-id="774d2-p106">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="774d2-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="774d2-147">応答</span><span class="sxs-lookup"><span data-stu-id="774d2-147">Response</span></span>

<span data-ttu-id="774d2-p107">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="774d2-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="774d2-150">例</span><span class="sxs-lookup"><span data-stu-id="774d2-150">Example</span></span>
<span data-ttu-id="774d2-151">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="774d2-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="774d2-152">要求</span><span class="sxs-lookup"><span data-stu-id="774d2-152">Request</span></span>
<span data-ttu-id="774d2-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="774d2-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="774d2-154">応答</span><span class="sxs-lookup"><span data-stu-id="774d2-154">Response</span></span>
<span data-ttu-id="774d2-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="774d2-155">Here is an example of the response.</span></span> 
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