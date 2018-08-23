# <a name="operation-resource-type"></a><span data-ttu-id="42bc5-101">操作リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42bc5-101">operation resource type</span></span>

<span data-ttu-id="42bc5-102">実行時間の長い操作の状態。</span><span class="sxs-lookup"><span data-stu-id="42bc5-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42bc5-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42bc5-103">JSON representation</span></span>

<span data-ttu-id="42bc5-104">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42bc5-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="42bc5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42bc5-105">Properties</span></span>
| <span data-ttu-id="42bc5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42bc5-106">Property</span></span>     | <span data-ttu-id="42bc5-107">型</span><span class="sxs-lookup"><span data-stu-id="42bc5-107">Type</span></span>   |<span data-ttu-id="42bc5-108">説明</span><span class="sxs-lookup"><span data-stu-id="42bc5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42bc5-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42bc5-109">createdDateTime</span></span>| <span data-ttu-id="42bc5-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bc5-110">DateTimeOffset</span></span> |<span data-ttu-id="42bc5-111">操作の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="42bc5-111">The start time of the operation.</span></span>|
|<span data-ttu-id="42bc5-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="42bc5-112">lastActionDateTime</span></span>| <span data-ttu-id="42bc5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bc5-113">DateTimeOffset</span></span> |<span data-ttu-id="42bc5-114">操作で最後に操作が行われた時間。</span><span class="sxs-lookup"><span data-stu-id="42bc5-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="42bc5-115">状態</span><span class="sxs-lookup"><span data-stu-id="42bc5-115">status</span></span>|<span data-ttu-id="42bc5-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="42bc5-116">operationStatus</span></span>|<span data-ttu-id="42bc5-117">操作の現在の状態: `notStarted`、`running`、`completed`、 `failed`</span><span class="sxs-lookup"><span data-stu-id="42bc5-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
