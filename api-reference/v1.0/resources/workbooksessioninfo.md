# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="a4700-101">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="a4700-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="a4700-102">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a4700-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a4700-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4700-103">JSON representation</span></span>

<span data-ttu-id="a4700-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a4700-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="a4700-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4700-105">Properties</span></span>

| <span data-ttu-id="a4700-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4700-106">Property</span></span> | <span data-ttu-id="a4700-107">型</span><span class="sxs-lookup"><span data-stu-id="a4700-107">Type</span></span>  | <span data-ttu-id="a4700-108">説明</span><span class="sxs-lookup"><span data-stu-id="a4700-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="a4700-109">id</span><span class="sxs-lookup"><span data-stu-id="a4700-109">id</span></span>  | <span data-ttu-id="a4700-110">string</span><span class="sxs-lookup"><span data-stu-id="a4700-110">string</span></span> | <span data-ttu-id="a4700-111">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="a4700-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="a4700-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="a4700-112">persistChanges</span></span> | <span data-ttu-id="a4700-113">string</span><span class="sxs-lookup"><span data-stu-id="a4700-113">string</span></span> |  <span data-ttu-id="a4700-114">`true`: 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="a4700-114">`true` for persistent session.</span></span> <span data-ttu-id="a4700-115">`false`: 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="a4700-115">`false` for non-persistent session (view mode)</span></span> |

