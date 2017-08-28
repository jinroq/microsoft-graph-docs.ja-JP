# <a name="resource-resource-type"></a><span data-ttu-id="0d065-101">resource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d065-101">resource resource type</span></span>

<span data-ttu-id="0d065-102">イメージまたは OneNote のページ上の他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="0d065-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="0d065-103">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d065-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="0d065-104">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="0d065-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="0d065-105">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="0d065-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="0d065-106">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0d065-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="0d065-107">`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0d065-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="0d065-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d065-108">Properties</span></span>
<span data-ttu-id="0d065-109">なし</span><span class="sxs-lookup"><span data-stu-id="0d065-109">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0d065-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d065-110">Relationships</span></span>
<span data-ttu-id="0d065-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0d065-111">None.</span></span>


## <a name="methods"></a><span data-ttu-id="0d065-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d065-112">Methods</span></span>
| <span data-ttu-id="0d065-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d065-113">Method</span></span>           | <span data-ttu-id="0d065-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d065-114">Return Type</span></span>    |<span data-ttu-id="0d065-115">説明</span><span class="sxs-lookup"><span data-stu-id="0d065-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d065-116">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="0d065-116">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="0d065-117">Stream</span><span class="sxs-lookup"><span data-stu-id="0d065-117">Stream</span></span> |<span data-ttu-id="0d065-118">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="0d065-118">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->