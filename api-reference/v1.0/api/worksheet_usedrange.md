# <a name="worksheet-usedrange"></a><span data-ttu-id="fb5f7-101">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="fb5f7-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="fb5f7-p101">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb5f7-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb5f7-104">Permissions</span></span>
<span data-ttu-id="fb5f7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb5f7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb5f7-107">Permission type</span></span>      | <span data-ttu-id="fb5f7-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb5f7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb5f7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb5f7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fb5f7-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb5f7-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb5f7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb5f7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb5f7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-112">Not supported.</span></span>    |
|<span data-ttu-id="fb5f7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb5f7-113">Application</span></span> | <span data-ttu-id="fb5f7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb5f7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb5f7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="parameters"></a><span data-ttu-id="fb5f7-116">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb5f7-116">Parameters</span></span>
<span data-ttu-id="fb5f7-117">要求 URL でオプション パラメーターを提供することがあります。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-117">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="fb5f7-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb5f7-118">Parameter</span></span>    | <span data-ttu-id="fb5f7-119">型</span><span class="sxs-lookup"><span data-stu-id="fb5f7-119">Type</span></span>   |<span data-ttu-id="fb5f7-120">説明</span><span class="sxs-lookup"><span data-stu-id="fb5f7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb5f7-121">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="fb5f7-121">valuesOnly</span></span>|<span data-ttu-id="fb5f7-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="fb5f7-122">Boolean</span></span>|<span data-ttu-id="fb5f7-p103">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p103">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fb5f7-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb5f7-125">Request headers</span></span>
| <span data-ttu-id="fb5f7-126">名前</span><span class="sxs-lookup"><span data-stu-id="fb5f7-126">Name</span></span>       | <span data-ttu-id="fb5f7-127">説明</span><span class="sxs-lookup"><span data-stu-id="fb5f7-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb5f7-128">承認</span><span class="sxs-lookup"><span data-stu-id="fb5f7-128">Authorization</span></span>  | <span data-ttu-id="fb5f7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb5f7-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb5f7-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb5f7-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="fb5f7-134">応答</span><span class="sxs-lookup"><span data-stu-id="fb5f7-134">Response</span></span>

<span data-ttu-id="fb5f7-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb5f7-136">例</span><span class="sxs-lookup"><span data-stu-id="fb5f7-136">Example</span></span>
<span data-ttu-id="fb5f7-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-137">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fb5f7-138">要求</span><span class="sxs-lookup"><span data-stu-id="fb5f7-138">Request</span></span>
<span data-ttu-id="fb5f7-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="fb5f7-140">応答</span><span class="sxs-lookup"><span data-stu-id="fb5f7-140">Response</span></span>
<span data-ttu-id="fb5f7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="fb5f7-144">代わりに、この関数はオプションの `valuesOnly` パラメーターを呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-144">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="fb5f7-145">要求</span><span class="sxs-lookup"><span data-stu-id="fb5f7-145">Request</span></span>
<span data-ttu-id="fb5f7-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="fb5f7-147">応答</span><span class="sxs-lookup"><span data-stu-id="fb5f7-147">Response</span></span>
<span data-ttu-id="fb5f7-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fb5f7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
