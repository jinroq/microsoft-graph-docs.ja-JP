# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="15ebd-101">onenoteEntityBaseModel リソース</span><span class="sxs-lookup"><span data-stu-id="15ebd-101">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="15ebd-102">OneNote のエンティティの基本データ型です。</span><span class="sxs-lookup"><span data-stu-id="15ebd-102">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15ebd-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15ebd-103">JSON representation</span></span>

<span data-ttu-id="15ebd-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15ebd-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="15ebd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15ebd-105">Properties</span></span>
| <span data-ttu-id="15ebd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15ebd-106">Property</span></span>     | <span data-ttu-id="15ebd-107">型</span><span class="sxs-lookup"><span data-stu-id="15ebd-107">Type</span></span>   |<span data-ttu-id="15ebd-108">説明</span><span class="sxs-lookup"><span data-stu-id="15ebd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15ebd-109">self</span><span class="sxs-lookup"><span data-stu-id="15ebd-109">self</span></span>|<span data-ttu-id="15ebd-110">String</span><span class="sxs-lookup"><span data-stu-id="15ebd-110">String</span></span>|<span data-ttu-id="15ebd-p101">ページに関する詳細情報を入手できるエンドポイント。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="15ebd-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->