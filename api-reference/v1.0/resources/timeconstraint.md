# <a name="timeconstraint-resource-type"></a><span data-ttu-id="c293b-101">timeConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c293b-101">timeConstraint resource type</span></span>

<span data-ttu-id="c293b-102">指定したアクティビティの性質と空き時間帯に従って、会議の日時の候補を、特定の時間と曜日に限定します。</span><span class="sxs-lookup"><span data-stu-id="c293b-102">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c293b-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c293b-103">JSON representation</span></span>

<span data-ttu-id="c293b-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c293b-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="c293b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c293b-105">Properties</span></span>
| <span data-ttu-id="c293b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c293b-106">Property</span></span>     | <span data-ttu-id="c293b-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="c293b-107">Type</span></span>   |<span data-ttu-id="c293b-108">説明</span><span class="sxs-lookup"><span data-stu-id="c293b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c293b-109">activityDomain</span><span class="sxs-lookup"><span data-stu-id="c293b-109">activityDomain</span></span>|<span data-ttu-id="c293b-110">activityDomain</span><span class="sxs-lookup"><span data-stu-id="c293b-110">activityDomain</span></span>|<span data-ttu-id="c293b-111">アクティビティの性質です (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="c293b-111">The nature of the activity, optional. Possible values are: , , , or .</span></span> <span data-ttu-id="c293b-112">指定できる値は、 `work`、`personal`、`unrestricted`、または `unknown` です。</span><span class="sxs-lookup"><span data-stu-id="c293b-112">The possible values are  `work`,  `personal`,  `unrestricted`, or  `unknown`.</span></span>|
|<span data-ttu-id="c293b-113">timeslots</span><span class="sxs-lookup"><span data-stu-id="c293b-113">timeslots</span></span>|<span data-ttu-id="c293b-114">[timeSlot](timeslot.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c293b-114">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="c293b-115">期間の配列。</span><span class="sxs-lookup"><span data-stu-id="c293b-115">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
