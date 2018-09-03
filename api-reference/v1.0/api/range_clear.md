# <a name="range-clear"></a><span data-ttu-id="3cf6a-101">範囲: クリア</span><span class="sxs-lookup"><span data-stu-id="3cf6a-101">Range: clear</span></span>

<span data-ttu-id="3cf6a-102">範囲の値、書式、塗りつぶし、罫線などをクリアします。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-102">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="3cf6a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3cf6a-103">Permissions</span></span>
<span data-ttu-id="3cf6a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3cf6a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cf6a-106">Permission type</span></span>      | <span data-ttu-id="3cf6a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cf6a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf6a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cf6a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf6a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cf6a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3cf6a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cf6a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf6a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-111">Not supported.</span></span>    |
|<span data-ttu-id="3cf6a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cf6a-112">Application</span></span> | <span data-ttu-id="3cf6a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cf6a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cf6a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="3cf6a-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cf6a-115">Request headers</span></span>
| <span data-ttu-id="3cf6a-116">名前</span><span class="sxs-lookup"><span data-stu-id="3cf6a-116">Name</span></span>       | <span data-ttu-id="3cf6a-117">説明</span><span class="sxs-lookup"><span data-stu-id="3cf6a-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3cf6a-118">承認</span><span class="sxs-lookup"><span data-stu-id="3cf6a-118">Authorization</span></span>  | <span data-ttu-id="3cf6a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cf6a-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3cf6a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="3cf6a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cf6a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cf6a-124">Request body</span></span>
<span data-ttu-id="3cf6a-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3cf6a-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3cf6a-126">Parameter</span></span>    | <span data-ttu-id="3cf6a-127">型</span><span class="sxs-lookup"><span data-stu-id="3cf6a-127">Type</span></span>   |<span data-ttu-id="3cf6a-128">説明</span><span class="sxs-lookup"><span data-stu-id="3cf6a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cf6a-129">applyTo</span><span class="sxs-lookup"><span data-stu-id="3cf6a-129">applyTo</span></span>|<span data-ttu-id="3cf6a-130">文字列</span><span class="sxs-lookup"><span data-stu-id="3cf6a-130">string</span></span>|<span data-ttu-id="3cf6a-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-131">Optional.</span></span> <span data-ttu-id="3cf6a-132">クリア アクションの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-132">Optional. Determines the type of clear action.  Possible values are: , , .</span></span>  <span data-ttu-id="3cf6a-133">使用可能な値: `All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-133">The possible values are `All`, `Formats`, or `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="3cf6a-134">応答</span><span class="sxs-lookup"><span data-stu-id="3cf6a-134">Response</span></span>

<span data-ttu-id="3cf6a-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf6a-137">例</span><span class="sxs-lookup"><span data-stu-id="3cf6a-137">Example</span></span>
<span data-ttu-id="3cf6a-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3cf6a-139">要求</span><span class="sxs-lookup"><span data-stu-id="3cf6a-139">Request</span></span>
<span data-ttu-id="3cf6a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="3cf6a-141">応答</span><span class="sxs-lookup"><span data-stu-id="3cf6a-141">Response</span></span>
<span data-ttu-id="3cf6a-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3cf6a-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->