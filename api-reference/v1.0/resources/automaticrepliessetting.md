# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="4a362-101">automaticRepliesSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a362-101">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="4a362-p101">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。</span><span class="sxs-lookup"><span data-stu-id="4a362-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="4a362-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a362-104">Properties</span></span>
| <span data-ttu-id="4a362-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a362-105">Property</span></span>     | <span data-ttu-id="4a362-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="4a362-106">Type</span></span>   |<span data-ttu-id="4a362-107">説明</span><span class="sxs-lookup"><span data-stu-id="4a362-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a362-108">externalAudience</span><span class="sxs-lookup"><span data-stu-id="4a362-108">externalAudience</span></span>|<span data-ttu-id="4a362-109">ExternalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="4a362-109">ExternalAudienceScope</span></span>| <span data-ttu-id="4a362-110">**Status** が `AlwaysEnabled` または `Scheduled` の場合に、**ExternalReplyMessage** を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。</span><span class="sxs-lookup"><span data-stu-id="4a362-110">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="4a362-111">使用可能な値: `none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="4a362-111">The possible values are `none`, `contactsOnly`, or `all`.</span></span>|
|<span data-ttu-id="4a362-112">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="4a362-112">externalReplyMessage</span></span>|<span data-ttu-id="4a362-113">文字列</span><span class="sxs-lookup"><span data-stu-id="4a362-113">string</span></span>|<span data-ttu-id="4a362-114">**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="4a362-114">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="4a362-115">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="4a362-115">internalReplyMessage</span></span>|<span data-ttu-id="4a362-116">文字列</span><span class="sxs-lookup"><span data-stu-id="4a362-116">string</span></span>|<span data-ttu-id="4a362-117">**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。</span><span class="sxs-lookup"><span data-stu-id="4a362-117">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="4a362-118">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="4a362-118">scheduledEndDateTime</span></span>|[<span data-ttu-id="4a362-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4a362-119">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="4a362-120">**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="4a362-120">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="4a362-121">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="4a362-121">scheduledStartDateTime</span></span>|[<span data-ttu-id="4a362-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4a362-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="4a362-123">**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="4a362-123">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="4a362-124">状態</span><span class="sxs-lookup"><span data-stu-id="4a362-124">status</span></span>|<span data-ttu-id="4a362-125">AutomaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="4a362-125">AutomaticRepliesStatus</span></span>|<span data-ttu-id="4a362-126">自動応答の構成状態です。</span><span class="sxs-lookup"><span data-stu-id="4a362-126">Configurations status for automatic replies. Possible values are: , , .</span></span> <span data-ttu-id="4a362-127">使用可能な値: `disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="4a362-127">The possible values are `disabled`, `alwaysEnabled`, or `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a362-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a362-128">JSON representation</span></span>

<span data-ttu-id="4a362-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a362-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
