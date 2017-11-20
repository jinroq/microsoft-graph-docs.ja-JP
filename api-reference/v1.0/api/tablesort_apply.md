# <a name="tablesort-apply"></a><span data-ttu-id="76afd-101">TableSort: apply　</span><span class="sxs-lookup"><span data-stu-id="76afd-101">TableSort: apply</span></span>

<span data-ttu-id="76afd-102">並べ替え操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="76afd-102">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="76afd-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76afd-103">Permissions</span></span>
<span data-ttu-id="76afd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76afd-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76afd-106">Permission type</span></span>      | <span data-ttu-id="76afd-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76afd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76afd-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76afd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="76afd-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76afd-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="76afd-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76afd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76afd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76afd-111">Not supported.</span></span>    |
|<span data-ttu-id="76afd-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76afd-112">Application</span></span> | <span data-ttu-id="76afd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76afd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76afd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76afd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="76afd-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76afd-115">Request headers</span></span>
| <span data-ttu-id="76afd-116">名前</span><span class="sxs-lookup"><span data-stu-id="76afd-116">Name</span></span>       | <span data-ttu-id="76afd-117">説明</span><span class="sxs-lookup"><span data-stu-id="76afd-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="76afd-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="76afd-118">Authorization</span></span>  | <span data-ttu-id="76afd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76afd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76afd-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76afd-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="76afd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="76afd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76afd-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="76afd-124">Request body</span></span>
<span data-ttu-id="76afd-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="76afd-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76afd-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="76afd-126">Parameter</span></span>    | <span data-ttu-id="76afd-127">型</span><span class="sxs-lookup"><span data-stu-id="76afd-127">Type</span></span>   |<span data-ttu-id="76afd-128">説明</span><span class="sxs-lookup"><span data-stu-id="76afd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76afd-129">fields</span><span class="sxs-lookup"><span data-stu-id="76afd-129">fields</span></span>|<span data-ttu-id="76afd-130">SortField</span><span class="sxs-lookup"><span data-stu-id="76afd-130">SortField</span></span>|<span data-ttu-id="76afd-131">並べ替えに使用する条件の一覧。</span><span class="sxs-lookup"><span data-stu-id="76afd-131">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="76afd-132">matchCase</span><span class="sxs-lookup"><span data-stu-id="76afd-132">matchCase</span></span>|<span data-ttu-id="76afd-133">boolean</span><span class="sxs-lookup"><span data-stu-id="76afd-133">boolean</span></span>|<span data-ttu-id="76afd-p104">省略可能。大文字小文字の区別が文字列の順序に影響を与えるかどうか。</span><span class="sxs-lookup"><span data-stu-id="76afd-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="76afd-136">method</span><span class="sxs-lookup"><span data-stu-id="76afd-136">method</span></span>|<span data-ttu-id="76afd-137">string</span><span class="sxs-lookup"><span data-stu-id="76afd-137">string</span></span>|<span data-ttu-id="76afd-p105">省略可能。中国語文字に使用される順序付けの方法です。可能な値は、`PinYin`、`StrokeCount` です。</span><span class="sxs-lookup"><span data-stu-id="76afd-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="76afd-141">応答</span><span class="sxs-lookup"><span data-stu-id="76afd-141">Response</span></span>

<span data-ttu-id="76afd-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="76afd-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76afd-144">例</span><span class="sxs-lookup"><span data-stu-id="76afd-144">Example</span></span>
<span data-ttu-id="76afd-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="76afd-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="76afd-146">要求</span><span class="sxs-lookup"><span data-stu-id="76afd-146">Request</span></span>
<span data-ttu-id="76afd-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76afd-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="76afd-148">応答</span><span class="sxs-lookup"><span data-stu-id="76afd-148">Response</span></span>
<span data-ttu-id="76afd-149">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="76afd-149">Here is an example of the response.</span></span> 
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