# <a name="listitemversion-resource-type"></a><span data-ttu-id="6c4af-101">ListItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c4af-101">ListItemVersion resource type</span></span>

<span data-ttu-id="6c4af-102">**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="6c4af-102">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="6c4af-103">ListItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="6c4af-103">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="6c4af-104">listItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c4af-104">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="6c4af-105">共通タスク</span><span class="sxs-lookup"><span data-stu-id="6c4af-105">Common task</span></span>             |         <span data-ttu-id="6c4af-106">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="6c4af-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="6c4af-107">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="6c4af-107">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="6c4af-108">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="6c4af-108">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="6c4af-109">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="6c4af-109">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem_list_versions.md
[version-get]: ../api/listitemversion_get.md
[version-restore]: ../api/listitemversion_restore.md


## <a name="json-representation"></a><span data-ttu-id="6c4af-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c4af-110">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="6c4af-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c4af-111">Properties</span></span>

|      <span data-ttu-id="6c4af-112">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6c4af-112">Property name</span></span>       |                         <span data-ttu-id="6c4af-113">型</span><span class="sxs-lookup"><span data-stu-id="6c4af-113">Type</span></span>                         |                               <span data-ttu-id="6c4af-114">説明</span><span class="sxs-lookup"><span data-stu-id="6c4af-114">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="6c4af-115">**id**</span><span class="sxs-lookup"><span data-stu-id="6c4af-115">**id**</span></span>                   | <span data-ttu-id="6c4af-116">string</span><span class="sxs-lookup"><span data-stu-id="6c4af-116">string</span></span>                                               | <span data-ttu-id="6c4af-117">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="6c4af-117">The ID of the version.</span></span> <span data-ttu-id="6c4af-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c4af-118">Read-only.</span></span>                                       |
| <span data-ttu-id="6c4af-119">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="6c4af-119">**lastModifiedBy**</span></span>       | [<span data-ttu-id="6c4af-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6c4af-120">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="6c4af-121">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="6c4af-121">Identity of the user which last modified the version.</span></span> <span data-ttu-id="6c4af-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c4af-122">Read-only.</span></span>        |
| <span data-ttu-id="6c4af-123">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6c4af-123">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="6c4af-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4af-124">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="6c4af-125">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="6c4af-125">Date and time the version was last modified.</span></span> <span data-ttu-id="6c4af-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c4af-126">Read-only.</span></span>                 |
| <span data-ttu-id="6c4af-127">**published**</span><span class="sxs-lookup"><span data-stu-id="6c4af-127">**published**</span></span>            | [<span data-ttu-id="6c4af-128">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6c4af-128">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="6c4af-129">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="6c4af-129">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="6c4af-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c4af-130">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="6c4af-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c4af-131">Relationships</span></span>

<span data-ttu-id="6c4af-132">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="6c4af-132">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="6c4af-133">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="6c4af-133">Relationship name</span></span> |                      <span data-ttu-id="6c4af-134">種類</span><span class="sxs-lookup"><span data-stu-id="6c4af-134">Type</span></span>                      |                               <span data-ttu-id="6c4af-135">説明</span><span class="sxs-lookup"><span data-stu-id="6c4af-135">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="6c4af-136">**fields**</span><span class="sxs-lookup"><span data-stu-id="6c4af-136">**fields**</span></span>        | [<span data-ttu-id="6c4af-137">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="6c4af-137">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="6c4af-138">このバージョンのリスト アイテムの、フィールドと値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="6c4af-138">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
