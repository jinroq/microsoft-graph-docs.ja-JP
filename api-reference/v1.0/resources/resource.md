# <a name="onenoteresource-resource-type"></a><span data-ttu-id="88846-101">OneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88846-101">OneNoteResource resource type</span></span>

<span data-ttu-id="88846-102">OneNote ページ上の画像または 他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="88846-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="88846-103">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88846-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="88846-104">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="88846-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="88846-105">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="88846-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="88846-106">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="88846-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="88846-107">タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。`object`</span><span class="sxs-lookup"><span data-stu-id="88846-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="88846-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88846-108">Properties</span></span>

| <span data-ttu-id="88846-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88846-109">Property</span></span>             | <span data-ttu-id="88846-110">タイプ</span><span class="sxs-lookup"><span data-stu-id="88846-110">Type</span></span>            | <span data-ttu-id="88846-111">説明</span><span class="sxs-lookup"><span data-stu-id="88846-111">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="88846-112">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="88846-112">content</span></span>              | <span data-ttu-id="88846-113">ストリーム</span><span class="sxs-lookup"><span data-stu-id="88846-113">Stream</span></span>          | <span data-ttu-id="88846-114">ストリーム</span><span class="sxs-lookup"><span data-stu-id="88846-114">The content stream.</span></span>
| <span data-ttu-id="88846-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="88846-115">contentUrl</span></span>           | <span data-ttu-id="88846-116">文字列 (URL)</span><span class="sxs-lookup"><span data-stu-id="88846-116">string (url)</span></span>    | <span data-ttu-id="88846-117">コンテンツをダウンロードするための URL</span><span class="sxs-lookup"><span data-stu-id="88846-117">The URL for the page's HTML content.  Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="88846-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="88846-118">Relationships</span></span>
<span data-ttu-id="88846-119">なし。</span><span class="sxs-lookup"><span data-stu-id="88846-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="88846-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="88846-120">Methods</span></span>
| <span data-ttu-id="88846-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="88846-121">Method</span></span>           | <span data-ttu-id="88846-122">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="88846-122">Return Type</span></span>    |<span data-ttu-id="88846-123">説明</span><span class="sxs-lookup"><span data-stu-id="88846-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88846-124">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="88846-124">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="88846-125">ストリーム</span><span class="sxs-lookup"><span data-stu-id="88846-125">Stream</span></span> |<span data-ttu-id="88846-126">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="88846-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->