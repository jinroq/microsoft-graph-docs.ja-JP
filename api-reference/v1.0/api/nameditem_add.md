# <a name="add-named-item"></a><span data-ttu-id="7c78d-101">名前付きアイテムの追加</span><span class="sxs-lookup"><span data-stu-id="7c78d-101">Add Named Item</span></span>

<span data-ttu-id="7c78d-102">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="7c78d-102">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c78d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c78d-103">Permissions</span></span>
<span data-ttu-id="7c78d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c78d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c78d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c78d-106">Permission type</span></span>      | <span data-ttu-id="7c78d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c78d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c78d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c78d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7c78d-109">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c78d-109">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="7c78d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c78d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c78d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c78d-111">Not supported.</span></span>    |
|<span data-ttu-id="7c78d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c78d-112">Application</span></span> | <span data-ttu-id="7c78d-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c78d-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c78d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c78d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="7c78d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c78d-115">Request headers</span></span>
| <span data-ttu-id="7c78d-116">名前</span><span class="sxs-lookup"><span data-stu-id="7c78d-116">Name</span></span>       | <span data-ttu-id="7c78d-117">説明</span><span class="sxs-lookup"><span data-stu-id="7c78d-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c78d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c78d-118">Authorization</span></span>  | <span data-ttu-id="7c78d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c78d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c78d-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c78d-121">Request body</span></span>
<span data-ttu-id="7c78d-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7c78d-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c78d-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c78d-123">Parameter</span></span>    | <span data-ttu-id="7c78d-124">型</span><span class="sxs-lookup"><span data-stu-id="7c78d-124">Type</span></span>   |<span data-ttu-id="7c78d-125">説明</span><span class="sxs-lookup"><span data-stu-id="7c78d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c78d-126">name</span><span class="sxs-lookup"><span data-stu-id="7c78d-126">name</span></span>|<span data-ttu-id="7c78d-127">string</span><span class="sxs-lookup"><span data-stu-id="7c78d-127">string</span></span>|<span data-ttu-id="7c78d-128">名前付きの項目の名前。</span><span class="sxs-lookup"><span data-stu-id="7c78d-128">The name of the named item.</span></span>|
|<span data-ttu-id="7c78d-129">reference</span><span class="sxs-lookup"><span data-stu-id="7c78d-129">reference</span></span>|<span data-ttu-id="7c78d-130">string</span><span class="sxs-lookup"><span data-stu-id="7c78d-130">string</span></span>|<span data-ttu-id="7c78d-131">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="7c78d-131">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="7c78d-132">comment</span><span class="sxs-lookup"><span data-stu-id="7c78d-132">comment</span></span>|<span data-ttu-id="7c78d-133">string</span><span class="sxs-lookup"><span data-stu-id="7c78d-133">string</span></span>|<span data-ttu-id="7c78d-134">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="7c78d-134">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="7c78d-135">応答</span><span class="sxs-lookup"><span data-stu-id="7c78d-135">Response</span></span>

<span data-ttu-id="7c78d-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [NamedItem](../resources/NamedItem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c78d-136">If successful, this method returns `200 OK` response code and [NamedItem](../resources/NamedItem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="7c78d-137">例</span><span class="sxs-lookup"><span data-stu-id="7c78d-137">Example</span></span>
<span data-ttu-id="7c78d-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7c78d-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7c78d-139">要求</span><span class="sxs-lookup"><span data-stu-id="7c78d-139">Request</span></span>
<span data-ttu-id="7c78d-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c78d-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="7c78d-141">応答</span><span class="sxs-lookup"><span data-stu-id="7c78d-141">Response</span></span>
<span data-ttu-id="7c78d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c78d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
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
