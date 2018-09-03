# <a name="baseitemversion-resource-type"></a><span data-ttu-id="9271d-101">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9271d-101">BaseItemVersion resource type</span></span>

<span data-ttu-id="9271d-102">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="9271d-102">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9271d-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9271d-103">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="9271d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9271d-104">Properties</span></span>

|      <span data-ttu-id="9271d-105">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9271d-105">Property name</span></span>       |                         <span data-ttu-id="9271d-106">型</span><span class="sxs-lookup"><span data-stu-id="9271d-106">Type</span></span>                         |                               <span data-ttu-id="9271d-107">説明</span><span class="sxs-lookup"><span data-stu-id="9271d-107">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="9271d-108">**ID**</span><span class="sxs-lookup"><span data-stu-id="9271d-108">**id**</span></span>                   | <span data-ttu-id="9271d-109">文字列</span><span class="sxs-lookup"><span data-stu-id="9271d-109">string</span></span>                                               | <span data-ttu-id="9271d-110">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="9271d-110">The ID of the version.</span></span> <span data-ttu-id="9271d-111">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9271d-111">Read-only.</span></span>                                       |
| <span data-ttu-id="9271d-112">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="9271d-112">**lastModifiedBy**</span></span>       | [<span data-ttu-id="9271d-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="9271d-113">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="9271d-114">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="9271d-114">Identity of the user which last modified the version.</span></span> <span data-ttu-id="9271d-115">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9271d-115">Read-only.</span></span>        |
| <span data-ttu-id="9271d-116">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="9271d-116">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="9271d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9271d-117">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="9271d-118">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="9271d-118">Date and time the version was last modified.</span></span> <span data-ttu-id="9271d-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9271d-119">Read-only.</span></span>                 |
| <span data-ttu-id="9271d-120">**出版物**</span><span class="sxs-lookup"><span data-stu-id="9271d-120">**publication**</span></span>          | [<span data-ttu-id="9271d-121">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="9271d-121">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="9271d-122">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="9271d-122">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="9271d-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9271d-123">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
