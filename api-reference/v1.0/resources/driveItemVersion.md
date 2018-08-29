# <a name="driveitemversion-resource-type"></a><span data-ttu-id="01cce-101">DriveItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01cce-101">DriveItemVersion resource type</span></span>

<span data-ttu-id="01cce-102">**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="01cce-102">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="01cce-103">DriveItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="01cce-103">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="01cce-104">driveItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="01cce-104">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="01cce-105">共通タスク</span><span class="sxs-lookup"><span data-stu-id="01cce-105">Common task</span></span>             |         <span data-ttu-id="01cce-106">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="01cce-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="01cce-107">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="01cce-107">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="01cce-108">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="01cce-108">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="01cce-109">[コンテンツの取得][content-get]</span><span class="sxs-lookup"><span data-stu-id="01cce-109">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="01cce-110">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="01cce-110">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem_list_versions.md
[version-get]: ../api/driveitemversion_get.md
[content-get]: ../api/driveitemversion_get_contents.md
[version-restore]: ../api/driveitemversion_restore.md

<span data-ttu-id="01cce-111">前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。</span><span class="sxs-lookup"><span data-stu-id="01cce-111">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01cce-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01cce-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="01cce-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01cce-113">Properties</span></span>

|      <span data-ttu-id="01cce-114">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="01cce-114">Property name</span></span>       |                         <span data-ttu-id="01cce-115">型</span><span class="sxs-lookup"><span data-stu-id="01cce-115">Type</span></span>                         |                               <span data-ttu-id="01cce-116">説明</span><span class="sxs-lookup"><span data-stu-id="01cce-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="01cce-117">**id**</span><span class="sxs-lookup"><span data-stu-id="01cce-117">**id**</span></span>                   | <span data-ttu-id="01cce-118">文字列</span><span class="sxs-lookup"><span data-stu-id="01cce-118">string</span></span>                                               | <span data-ttu-id="01cce-119">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="01cce-119">The ID of the version.</span></span> <span data-ttu-id="01cce-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="01cce-120">Read-only.</span></span>                                       |
| <span data-ttu-id="01cce-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="01cce-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="01cce-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="01cce-122">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="01cce-123">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="01cce-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="01cce-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="01cce-124">Read-only.</span></span>        |
| <span data-ttu-id="01cce-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="01cce-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="01cce-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01cce-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="01cce-127">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="01cce-127">Date and time the version was last modified.</span></span> <span data-ttu-id="01cce-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="01cce-128">Read-only.</span></span>                 |
| <span data-ttu-id="01cce-129">**publication**</span><span class="sxs-lookup"><span data-stu-id="01cce-129">**publication**</span></span>          | [<span data-ttu-id="01cce-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="01cce-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="01cce-131">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="01cce-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="01cce-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="01cce-132">Read-only.</span></span> |
| <span data-ttu-id="01cce-133">**size**</span><span class="sxs-lookup"><span data-stu-id="01cce-133">**size**</span></span>                 | <span data-ttu-id="01cce-134">Int64</span><span class="sxs-lookup"><span data-stu-id="01cce-134">Int64</span></span>                                                | <span data-ttu-id="01cce-135">アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。</span><span class="sxs-lookup"><span data-stu-id="01cce-135">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="01cce-136">**content**</span><span class="sxs-lookup"><span data-stu-id="01cce-136">**content**</span></span>              | <span data-ttu-id="01cce-137">ストリーム</span><span class="sxs-lookup"><span data-stu-id="01cce-137">Stream</span></span>                                               | <span data-ttu-id="01cce-138">項目のこのバージョンのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="01cce-138">Indicates the size of the content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
