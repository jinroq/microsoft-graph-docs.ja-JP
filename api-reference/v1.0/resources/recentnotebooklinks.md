# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="d6dc2-101">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="d6dc2-101">recentNotebookLinks resource type</span></span>

<span data-ttu-id="d6dc2-102">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="d6dc2-102">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="d6dc2-103">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="d6dc2-103">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d6dc2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6dc2-104">Properties</span></span>
| <span data-ttu-id="d6dc2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6dc2-105">Property</span></span>     | <span data-ttu-id="d6dc2-106">型</span><span class="sxs-lookup"><span data-stu-id="d6dc2-106">Type</span></span>   |<span data-ttu-id="d6dc2-107">説明</span><span class="sxs-lookup"><span data-stu-id="d6dc2-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6dc2-108">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d6dc2-108">oneNoteClientUrl</span></span>|[<span data-ttu-id="d6dc2-109">externalLink</span><span class="sxs-lookup"><span data-stu-id="d6dc2-109">externalLink</span></span>](externallink.md)|<span data-ttu-id="d6dc2-110">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="d6dc2-110">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d6dc2-111">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d6dc2-111">oneNoteWebUrl</span></span>|[<span data-ttu-id="d6dc2-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="d6dc2-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="d6dc2-113">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="d6dc2-113">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6dc2-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6dc2-114">JSON representation</span></span>

<span data-ttu-id="d6dc2-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6dc2-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
