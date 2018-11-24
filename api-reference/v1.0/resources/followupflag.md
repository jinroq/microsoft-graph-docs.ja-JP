# <a name="followupflag-resource-type"></a><span data-ttu-id="59e7e-101">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59e7e-101">followupFlag resource type</span></span>


<span data-ttu-id="59e7e-102">ユーザーが後でフォローするためのアイテムにフラグを設定できます。</span><span class="sxs-lookup"><span data-stu-id="59e7e-102">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="59e7e-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59e7e-103">Properties</span></span>
| <span data-ttu-id="59e7e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59e7e-104">Property</span></span>     | <span data-ttu-id="59e7e-105">型</span><span class="sxs-lookup"><span data-stu-id="59e7e-105">Type</span></span>   |<span data-ttu-id="59e7e-106">説明</span><span class="sxs-lookup"><span data-stu-id="59e7e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59e7e-107">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="59e7e-107">completedDateTime</span></span>|[<span data-ttu-id="59e7e-108">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="59e7e-108">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="59e7e-109">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="59e7e-109">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="59e7e-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="59e7e-110">dueDateTime</span></span>|<span data-ttu-id="59e7e-111">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="59e7e-111">**dateTimeTimeZone**</span></span>|<span data-ttu-id="59e7e-112">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="59e7e-112">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="59e7e-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="59e7e-113">flagStatus</span></span>|<span data-ttu-id="59e7e-114">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="59e7e-114">followupFlagStatus</span></span>|<span data-ttu-id="59e7e-115">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="59e7e-115">The status for follow-up for an item.</span></span> <span data-ttu-id="59e7e-116">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="59e7e-116">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="59e7e-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59e7e-117">startDateTime</span></span>|<span data-ttu-id="59e7e-118">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="59e7e-118">**dateTimeTimeZone**</span></span>|<span data-ttu-id="59e7e-119">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="59e7e-119">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59e7e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59e7e-120">JSON representation</span></span>

<span data-ttu-id="59e7e-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="59e7e-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
