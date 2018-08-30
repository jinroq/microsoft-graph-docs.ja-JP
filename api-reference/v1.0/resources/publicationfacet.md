# <a name="publicationfacet-resource-type"></a><span data-ttu-id="50475-101">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50475-101">PublicationFacet resource type</span></span>

<span data-ttu-id="50475-102">**publicationFacet **リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="50475-102">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50475-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50475-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="50475-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50475-104">Properties</span></span>

|   <span data-ttu-id="50475-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50475-105">Property</span></span>    |  <span data-ttu-id="50475-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="50475-106">Type</span></span>  | <span data-ttu-id="50475-107">説明</span><span class="sxs-lookup"><span data-stu-id="50475-107">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="50475-108">**level**</span><span class="sxs-lookup"><span data-stu-id="50475-108">**level**</span></span>     | <span data-ttu-id="50475-109">文字列</span><span class="sxs-lookup"><span data-stu-id="50475-109">String</span></span> | <span data-ttu-id="50475-110">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="50475-110">The state of publication for this document.</span></span> <span data-ttu-id="50475-111">または `checkout` のどちらかです。`published`</span><span class="sxs-lookup"><span data-stu-id="50475-111">Either `published` or `checkout`.</span></span> <span data-ttu-id="50475-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="50475-112">Read-only.</span></span>  |
| <span data-ttu-id="50475-113">**versionId**</span><span class="sxs-lookup"><span data-stu-id="50475-113">**versionId**</span></span> | <span data-ttu-id="50475-114">文字列</span><span class="sxs-lookup"><span data-stu-id="50475-114">String</span></span> | <span data-ttu-id="50475-115">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="50475-115">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="50475-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="50475-116">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
