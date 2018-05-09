# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="5848c-101">mailboxSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5848c-101">mailboxSettings resource type</span></span>

<span data-ttu-id="5848c-102">サインイン ユーザーのプライマリ メールボックスの設定。</span><span class="sxs-lookup"><span data-stu-id="5848c-102">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="5848c-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5848c-103">Properties</span></span>
| <span data-ttu-id="5848c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5848c-104">Property</span></span>     | <span data-ttu-id="5848c-105">型</span><span class="sxs-lookup"><span data-stu-id="5848c-105">Type</span></span>   |<span data-ttu-id="5848c-106">説明</span><span class="sxs-lookup"><span data-stu-id="5848c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5848c-107">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="5848c-107">archiveFolder</span></span>|<span data-ttu-id="5848c-108">string</span><span class="sxs-lookup"><span data-stu-id="5848c-108">string</span></span>|<span data-ttu-id="5848c-109">ユーザーのアーカイブ フォルダーのフォルダー ID。</span><span class="sxs-lookup"><span data-stu-id="5848c-109">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="5848c-110">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5848c-110">automaticRepliesSetting</span></span>|[<span data-ttu-id="5848c-111">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5848c-111">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="5848c-112">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="5848c-112">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="5848c-113">language</span><span class="sxs-lookup"><span data-stu-id="5848c-113">language</span></span>|[<span data-ttu-id="5848c-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="5848c-114">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="5848c-115">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="5848c-115">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="5848c-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="5848c-116">timeZone</span></span>|<span data-ttu-id="5848c-117">string</span><span class="sxs-lookup"><span data-stu-id="5848c-117">string</span></span>|<span data-ttu-id="5848c-118">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="5848c-118">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="5848c-119">workingHours</span><span class="sxs-lookup"><span data-stu-id="5848c-119">workingHours</span></span>|[<span data-ttu-id="5848c-120">workingHours</span><span class="sxs-lookup"><span data-stu-id="5848c-120">workingHours</span></span>](workinghours.md)|<span data-ttu-id="5848c-121">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="5848c-121">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5848c-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5848c-122">JSON representation</span></span>

<span data-ttu-id="5848c-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5848c-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->