# <a name="timestamp-resource-type"></a><span data-ttu-id="f4637-101">timestamp のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4637-101">timeStamp resource type</span></span>

<span data-ttu-id="f4637-102">時間のポイントの日付と時刻情報です。</span><span class="sxs-lookup"><span data-stu-id="f4637-102">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4637-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4637-103">JSON representation</span></span>

<span data-ttu-id="f4637-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f4637-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f4637-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4637-105">Properties</span></span>
| <span data-ttu-id="f4637-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4637-106">Property</span></span>       | <span data-ttu-id="f4637-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="f4637-107">Type</span></span>    |<span data-ttu-id="f4637-108">説明</span><span class="sxs-lookup"><span data-stu-id="f4637-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4637-109">date</span><span class="sxs-lookup"><span data-stu-id="f4637-109">date</span></span>|<span data-ttu-id="f4637-110">日付</span><span class="sxs-lookup"><span data-stu-id="f4637-110">Date</span></span>|<span data-ttu-id="f4637-111">タイムスタンプの日付部分。</span><span class="sxs-lookup"><span data-stu-id="f4637-111">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="f4637-112">time</span><span class="sxs-lookup"><span data-stu-id="f4637-112">time</span></span>|<span data-ttu-id="f4637-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f4637-113">TimeOfDay</span></span>|<span data-ttu-id="f4637-114">タイムスタンプの時刻部分。</span><span class="sxs-lookup"><span data-stu-id="f4637-114">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="f4637-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="f4637-115">timeZone</span></span>|<span data-ttu-id="f4637-116">文字列</span><span class="sxs-lookup"><span data-stu-id="f4637-116">String</span></span>|<span data-ttu-id="f4637-117">timestamp のタイム ゾーン部分。世界を 24 個の縦方向の領域に分けたうちのいずれかの領域です。</span><span class="sxs-lookup"><span data-stu-id="f4637-117">The time zone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->