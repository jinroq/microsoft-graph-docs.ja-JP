# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="ed307-101">automaticRepliesMailTips リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ed307-101">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="ed307-102">メールボックスで設定されている自動返信についての[メール ヒント](../resources/mailtips.md)。</span><span class="sxs-lookup"><span data-stu-id="ed307-102">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="ed307-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed307-103">Properties</span></span>
| <span data-ttu-id="ed307-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed307-104">Property</span></span>     | <span data-ttu-id="ed307-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="ed307-105">Type</span></span>   |<span data-ttu-id="ed307-106">説明</span><span class="sxs-lookup"><span data-stu-id="ed307-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="ed307-107">message</span><span class="sxs-lookup"><span data-stu-id="ed307-107">message</span></span> | <span data-ttu-id="ed307-108">文字列</span><span class="sxs-lookup"><span data-stu-id="ed307-108">String</span></span> | <span data-ttu-id="ed307-109">自動応答メッセージ。</span><span class="sxs-lookup"><span data-stu-id="ed307-109">The automatic reply message.</span></span> |
| <span data-ttu-id="ed307-110">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="ed307-110">messageLanguage</span></span> | [<span data-ttu-id="ed307-111">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ed307-111">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="ed307-112">自動応答メッセージの言語。</span><span class="sxs-lookup"><span data-stu-id="ed307-112">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="ed307-113">ScheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="ed307-113">ScheduledEndTime</span></span> | [<span data-ttu-id="ed307-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ed307-114">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="ed307-115">自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="ed307-115">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="ed307-116">ScheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="ed307-116">ScheduledStartTime</span></span> | [<span data-ttu-id="ed307-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ed307-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="ed307-118">自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="ed307-118">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed307-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ed307-119">JSON representation</span></span>

<span data-ttu-id="ed307-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ed307-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->