# <a name="customtimezone-resource-type"></a><span data-ttu-id="6a0fd-101">customTimeZone リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a0fd-101">customTimeZone resource type</span></span>

<span data-ttu-id="6a0fd-102">標準時から夏時間またはその逆への切り替えが標準となっていないタイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="6a0fd-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a0fd-103">Properties</span></span>
| <span data-ttu-id="6a0fd-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a0fd-104">Property</span></span>     | <span data-ttu-id="6a0fd-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="6a0fd-105">Type</span></span>   |<span data-ttu-id="6a0fd-106">説明</span><span class="sxs-lookup"><span data-stu-id="6a0fd-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6a0fd-107">bias</span><span class="sxs-lookup"><span data-stu-id="6a0fd-107">bias</span></span> | <span data-ttu-id="6a0fd-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="6a0fd-108">Edm.Int32</span></span> | <span data-ttu-id="6a0fd-109">タイム ゾーンの協定世界時 (UTC) からの時間オフセットです。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="6a0fd-110">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-110">This value is in minutes.</span></span> <span data-ttu-id="6a0fd-111">UTC より時間が進んでいるタイム　ゾーンには正のオフセット、UTC より時間が遅れているタイム ゾーンには負のオフセットを設定します。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="6a0fd-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="6a0fd-112">daylightOffset</span></span> | [<span data-ttu-id="6a0fd-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="6a0fd-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="6a0fd-114">タイム ゾーンが標準時から夏時間に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="6a0fd-115">name</span><span class="sxs-lookup"><span data-stu-id="6a0fd-115">name</span></span> | <span data-ttu-id="6a0fd-116">string</span><span class="sxs-lookup"><span data-stu-id="6a0fd-116">string</span></span> | <span data-ttu-id="6a0fd-117">カスタム タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="6a0fd-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="6a0fd-118">standardOffset</span></span> | [<span data-ttu-id="6a0fd-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="6a0fd-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="6a0fd-120">タイム ゾーンが夏時間から標準時に切り替わるタイミングを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6a0fd-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a0fd-121">JSON representation</span></span>

<span data-ttu-id="6a0fd-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a0fd-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->