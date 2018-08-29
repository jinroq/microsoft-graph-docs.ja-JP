# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="c3e0e-101">workbookSessionInfo リソース型</span><span class="sxs-lookup"><span data-stu-id="c3e0e-101">workbookSessionInfo resource type</span></span>

<span data-ttu-id="c3e0e-102">ブック セッションについての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c3e0e-102">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3e0e-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3e0e-103">JSON representation</span></span>

<span data-ttu-id="c3e0e-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c3e0e-104">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="c3e0e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3e0e-105">Properties</span></span>

| <span data-ttu-id="c3e0e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3e0e-106">Property</span></span> | <span data-ttu-id="c3e0e-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="c3e0e-107">Type</span></span>  | <span data-ttu-id="c3e0e-108">説明</span><span class="sxs-lookup"><span data-stu-id="c3e0e-108">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="c3e0e-109">ID</span><span class="sxs-lookup"><span data-stu-id="c3e0e-109">id</span></span>  | <span data-ttu-id="c3e0e-110">文字列</span><span class="sxs-lookup"><span data-stu-id="c3e0e-110">string</span></span> | <span data-ttu-id="c3e0e-111">ブック セッションの ID。</span><span class="sxs-lookup"><span data-stu-id="c3e0e-111">Id of the workbook session.</span></span> |
| <span data-ttu-id="c3e0e-112">persistChanges</span><span class="sxs-lookup"><span data-stu-id="c3e0e-112">persistChanges</span></span> | <span data-ttu-id="c3e0e-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="c3e0e-113">boolean</span></span> |  <span data-ttu-id="c3e0e-114">`true` : 永続セッションの場合。</span><span class="sxs-lookup"><span data-stu-id="c3e0e-114">`true` for persistent session.</span></span> <span data-ttu-id="c3e0e-115">`false` : 非永続セッション (表示モード) の場合。</span><span class="sxs-lookup"><span data-stu-id="c3e0e-115">`false` for non-persistent session (view mode)</span></span> |

