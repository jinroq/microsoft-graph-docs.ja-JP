# <a name="add-named-item-formulalocal"></a><span data-ttu-id="dae50-101">名前付きアイテム FormulaLocal の追加</span><span class="sxs-lookup"><span data-stu-id="dae50-101">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="dae50-102">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="dae50-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="dae50-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="dae50-103">Permissions</span></span>
<span data-ttu-id="dae50-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dae50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dae50-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dae50-106">Permission type</span></span>      | <span data-ttu-id="dae50-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="dae50-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dae50-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dae50-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dae50-109">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae50-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="dae50-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dae50-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dae50-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dae50-111">Not supported.</span></span>    |
|<span data-ttu-id="dae50-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dae50-112">Application</span></span> | <span data-ttu-id="dae50-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="dae50-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae50-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dae50-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="dae50-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dae50-115">Request headers</span></span>
| <span data-ttu-id="dae50-116">名前</span><span class="sxs-lookup"><span data-stu-id="dae50-116">Name</span></span>       | <span data-ttu-id="dae50-117">説明</span><span class="sxs-lookup"><span data-stu-id="dae50-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dae50-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="dae50-118">Authorization</span></span>  | <span data-ttu-id="dae50-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="dae50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dae50-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dae50-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="dae50-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="dae50-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae50-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="dae50-124">Request body</span></span>
<span data-ttu-id="dae50-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="dae50-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dae50-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="dae50-126">Parameter</span></span>    | <span data-ttu-id="dae50-127">Type</span><span class="sxs-lookup"><span data-stu-id="dae50-127">Type</span></span>   |<span data-ttu-id="dae50-128">説明</span><span class="sxs-lookup"><span data-stu-id="dae50-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dae50-129">name</span><span class="sxs-lookup"><span data-stu-id="dae50-129">name</span></span>|<span data-ttu-id="dae50-130">string</span><span class="sxs-lookup"><span data-stu-id="dae50-130">string</span></span>|<span data-ttu-id="dae50-131">名前付きのアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="dae50-131">The name of the named item.</span></span>|
|<span data-ttu-id="dae50-132">formula</span><span class="sxs-lookup"><span data-stu-id="dae50-132">formula</span></span>|<span data-ttu-id="dae50-133">string</span><span class="sxs-lookup"><span data-stu-id="dae50-133">string</span></span>|<span data-ttu-id="dae50-134">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="dae50-134">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="dae50-135">comment</span><span class="sxs-lookup"><span data-stu-id="dae50-135">comment</span></span>|<span data-ttu-id="dae50-136">string</span><span class="sxs-lookup"><span data-stu-id="dae50-136">string</span></span>|<span data-ttu-id="dae50-137">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="dae50-137">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="dae50-138">応答</span><span class="sxs-lookup"><span data-stu-id="dae50-138">Response</span></span>

<span data-ttu-id="dae50-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [NamedItem](../resources/NamedItem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dae50-139">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dae50-140">例</span><span class="sxs-lookup"><span data-stu-id="dae50-140">Example</span></span>
<span data-ttu-id="dae50-141">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="dae50-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dae50-142">要求</span><span class="sxs-lookup"><span data-stu-id="dae50-142">Request</span></span>
<span data-ttu-id="dae50-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dae50-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="dae50-144">応答</span><span class="sxs-lookup"><span data-stu-id="dae50-144">Response</span></span>
<span data-ttu-id="dae50-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dae50-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
    "visible": true
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
