# <a name="rangesort-apply"></a><span data-ttu-id="883c9-101">RangeSort: 適用</span><span class="sxs-lookup"><span data-stu-id="883c9-101">RangeSort: apply</span></span>

<span data-ttu-id="883c9-102">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="883c9-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="883c9-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="883c9-103">Permissions</span></span>
<span data-ttu-id="883c9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="883c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="883c9-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="883c9-106">Permission type</span></span>      | <span data-ttu-id="883c9-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="883c9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="883c9-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="883c9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="883c9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="883c9-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="883c9-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="883c9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="883c9-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883c9-111">Not supported.</span></span>    |
|<span data-ttu-id="883c9-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="883c9-112">Application</span></span> | <span data-ttu-id="883c9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="883c9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="883c9-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="883c9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="883c9-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="883c9-115">Request headers</span></span>
| <span data-ttu-id="883c9-116">名前</span><span class="sxs-lookup"><span data-stu-id="883c9-116">Name</span></span>       | <span data-ttu-id="883c9-117">説明</span><span class="sxs-lookup"><span data-stu-id="883c9-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="883c9-118">承認</span><span class="sxs-lookup"><span data-stu-id="883c9-118">Authorization</span></span>  | <span data-ttu-id="883c9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="883c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="883c9-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="883c9-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="883c9-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="883c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="883c9-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="883c9-124">Request body</span></span>
<span data-ttu-id="883c9-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="883c9-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="883c9-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="883c9-126">Parameter</span></span>    | <span data-ttu-id="883c9-127">型</span><span class="sxs-lookup"><span data-stu-id="883c9-127">Type</span></span>   |<span data-ttu-id="883c9-128">説明</span><span class="sxs-lookup"><span data-stu-id="883c9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="883c9-129">fields</span><span class="sxs-lookup"><span data-stu-id="883c9-129">fields</span></span>|<span data-ttu-id="883c9-130">WorkbookSortField コレクション</span><span class="sxs-lookup"><span data-stu-id="883c9-130">WorkbookSortField collection</span></span>|<span data-ttu-id="883c9-131">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="883c9-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="883c9-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="883c9-132">matchCase</span></span>|<span data-ttu-id="883c9-133">boolean</span><span class="sxs-lookup"><span data-stu-id="883c9-133">boolean</span></span>|<span data-ttu-id="883c9-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="883c9-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="883c9-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="883c9-136">hasHeaders</span></span>|<span data-ttu-id="883c9-137">boolean</span><span class="sxs-lookup"><span data-stu-id="883c9-137">boolean</span></span>|<span data-ttu-id="883c9-p105">省略可能。範囲にヘッダーがあるかどうか。</span><span class="sxs-lookup"><span data-stu-id="883c9-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="883c9-140">orientation</span><span class="sxs-lookup"><span data-stu-id="883c9-140">orientation</span></span>|<span data-ttu-id="883c9-141">string</span><span class="sxs-lookup"><span data-stu-id="883c9-141">string</span></span>|<span data-ttu-id="883c9-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="883c9-142">Optional.</span></span> <span data-ttu-id="883c9-143">操作が行または列の並べ替えを行なっているかどうか。</span><span class="sxs-lookup"><span data-stu-id="883c9-143">Optional. Whether the operation is sorting rows or columns.  Possible values are: , .</span></span>  <span data-ttu-id="883c9-144">可能な値は、`Rows`、`Columns` です。</span><span class="sxs-lookup"><span data-stu-id="883c9-144">The possible values are:</span></span>|
|<span data-ttu-id="883c9-145">method</span><span class="sxs-lookup"><span data-stu-id="883c9-145">method</span></span>|<span data-ttu-id="883c9-146">string</span><span class="sxs-lookup"><span data-stu-id="883c9-146">string</span></span>|<span data-ttu-id="883c9-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="883c9-147">Optional.</span></span> <span data-ttu-id="883c9-148">中国語の文字に使用される順序の指定方法です。</span><span class="sxs-lookup"><span data-stu-id="883c9-148">Optional. The ordering method used for Chinese characters.  Possible values are: , .</span></span>  <span data-ttu-id="883c9-149">可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="883c9-149">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="883c9-150">応答</span><span class="sxs-lookup"><span data-stu-id="883c9-150">Response</span></span>

<span data-ttu-id="883c9-p108">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="883c9-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="883c9-153">例</span><span class="sxs-lookup"><span data-stu-id="883c9-153">Example</span></span>
<span data-ttu-id="883c9-154">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="883c9-154">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="883c9-155">要求</span><span class="sxs-lookup"><span data-stu-id="883c9-155">Request</span></span>
<span data-ttu-id="883c9-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="883c9-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="883c9-157">応答</span><span class="sxs-lookup"><span data-stu-id="883c9-157">Response</span></span>
<span data-ttu-id="883c9-158">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="883c9-158">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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