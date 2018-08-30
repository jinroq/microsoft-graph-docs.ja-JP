# <a name="followupflag-resource-type"></a><span data-ttu-id="13cd5-101">followupFlag リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13cd5-101">followupFlag resource type</span></span>


<span data-ttu-id="13cd5-102">ユーザーが特定のアイテムを後でフォローアップできるよう、フラグを設定できます。</span><span class="sxs-lookup"><span data-stu-id="13cd5-102">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="13cd5-103">サポートされているアイテムには、[メッセージ](message.md)と[連絡先](contact.md)があります。</span><span class="sxs-lookup"><span data-stu-id="13cd5-103">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="13cd5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13cd5-104">Properties</span></span>
| <span data-ttu-id="13cd5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13cd5-105">Property</span></span>     | <span data-ttu-id="13cd5-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="13cd5-106">Type</span></span>   |<span data-ttu-id="13cd5-107">説明</span><span class="sxs-lookup"><span data-stu-id="13cd5-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13cd5-108">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="13cd5-108">completedDateTime</span></span>|[<span data-ttu-id="13cd5-109">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="13cd5-109">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="13cd5-110">フォローアップが終了した日時。</span><span class="sxs-lookup"><span data-stu-id="13cd5-110">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="13cd5-111">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="13cd5-111">dueDateTime</span></span>|<span data-ttu-id="13cd5-112">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="13cd5-112">**dateTimeTimeZone**</span></span>|<span data-ttu-id="13cd5-113">フォローアップが終了する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="13cd5-113">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="13cd5-114">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="13cd5-114">flagStatus</span></span>|<span data-ttu-id="13cd5-115">FollowupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="13cd5-115">FollowupFlagStatus</span></span>|<span data-ttu-id="13cd5-116">アイテムのフォローアップ状態。</span><span class="sxs-lookup"><span data-stu-id="13cd5-116">The status for follow-up for an item.</span></span> <span data-ttu-id="13cd5-117">可能な値は、`notFlagged`、`complete`、`flagged` です。</span><span class="sxs-lookup"><span data-stu-id="13cd5-117">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="13cd5-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="13cd5-118">startDateTime</span></span>|<span data-ttu-id="13cd5-119">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="13cd5-119">**dateTimeTimeZone**</span></span>|<span data-ttu-id="13cd5-120">フォローアップを開始する予定の日時。</span><span class="sxs-lookup"><span data-stu-id="13cd5-120">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13cd5-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13cd5-121">JSON representation</span></span>

<span data-ttu-id="13cd5-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="13cd5-122">Here is a JSON representation of the resource</span></span>

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
