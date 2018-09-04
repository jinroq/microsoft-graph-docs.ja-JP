# <a name="mailtips-resource-type"></a><span data-ttu-id="91597-101">mailTips リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91597-101">mailTips resource type</span></span>

<span data-ttu-id="91597-102">メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。</span><span class="sxs-lookup"><span data-stu-id="91597-102">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="91597-103">メッセージの受信者に対するj移動返信としての不在時のメッセージがその例です。</span><span class="sxs-lookup"><span data-stu-id="91597-103">Informative messages displayed to users while they are composing a message. For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="91597-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91597-104">Properties</span></span>
| <span data-ttu-id="91597-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91597-105">Property</span></span>     | <span data-ttu-id="91597-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="91597-106">Type</span></span>   |<span data-ttu-id="91597-107">説明</span><span class="sxs-lookup"><span data-stu-id="91597-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91597-108">AutomaticReplies</span><span class="sxs-lookup"><span data-stu-id="91597-108">AutomaticReplies</span></span> | [<span data-ttu-id="91597-109">AutomaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="91597-109">AutomaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="91597-110">受信者によって設定されている場合の自動応答に関するメールのヒント。</span><span class="sxs-lookup"><span data-stu-id="91597-110">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="91597-111">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="91597-111">CustomMailTip</span></span> | <span data-ttu-id="91597-112">文字列</span><span class="sxs-lookup"><span data-stu-id="91597-112">String</span></span> | <span data-ttu-id="91597-113">受信者のメールボックスに設定可能なカスタム メールのヒント。</span><span class="sxs-lookup"><span data-stu-id="91597-113">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="91597-114">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="91597-114">DeliveryRestricted</span></span>| <span data-ttu-id="91597-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="91597-115">Boolean</span></span> | <span data-ttu-id="91597-116">受信者のメールボックスが制限されているかどうか。たとえば、送信者の定義済みリストからのメッセージのみを受け付ける、送信者の定義済みリストからのメッセージを拒否する、または認証された送信者からのメッセージのみを受信するなどです。</span><span class="sxs-lookup"><span data-stu-id="91597-116">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="91597-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91597-117">emailAddress</span></span> | [<span data-ttu-id="91597-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91597-118">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="91597-119">メールヒントを取得する受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="91597-119">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="91597-120">エラー</span><span class="sxs-lookup"><span data-stu-id="91597-120">error</span></span> | [<span data-ttu-id="91597-121">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="91597-121">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="91597-122">[GetMailTips](../api/user_getmailtips.md) アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="91597-122">Errors that occur during the [GetMailTips](../api/user_getmailtips.md) action.</span></span> |
| <span data-ttu-id="91597-123">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="91597-123">ExternalMemberCount</span></span> | <span data-ttu-id="91597-124">Int32</span><span class="sxs-lookup"><span data-stu-id="91597-124">Int32</span></span> | <span data-ttu-id="91597-125">受信者が配布リストの場合は外部メンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="91597-125">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="91597-126">IsModerated</span><span class="sxs-lookup"><span data-stu-id="91597-126">IsModerated</span></span> |<span data-ttu-id="91597-127">ブール値</span><span class="sxs-lookup"><span data-stu-id="91597-127">Boolean</span></span>  | <span data-ttu-id="91597-p102">受信者へのメッセージ送信に承認が必要かどうか。たとえば、受信者が大規模な配布リストであり、モデレーターが配布リストに送信されたメッセージを承認するようにセットアップされている場合、または受信者へのメッセージの送信に受信者の上司の承認を必要とする場合などです。</span><span class="sxs-lookup"><span data-stu-id="91597-p102">Whether sending messages to the recipient requires approval. For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="91597-130">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="91597-130">MailboxFull</span></span> | <span data-ttu-id="91597-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="91597-131">Boolean</span></span> | <span data-ttu-id="91597-132">受信者のメールボックスのフル状態。</span><span class="sxs-lookup"><span data-stu-id="91597-132">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="91597-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="91597-133">MaxMessageSize</span></span> | <span data-ttu-id="91597-134">Int32</span><span class="sxs-lookup"><span data-stu-id="91597-134">Int32</span></span> | <span data-ttu-id="91597-135">受信者の組織またはメールボックスに対して構成されているメッセージの最大サイズ。</span><span class="sxs-lookup"><span data-stu-id="91597-135">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="91597-136">RecipientScope</span><span class="sxs-lookup"><span data-stu-id="91597-136">RecipientScope</span></span> | <span data-ttu-id="91597-137">文字列</span><span class="sxs-lookup"><span data-stu-id="91597-137">String</span></span> | <span data-ttu-id="91597-138">受信者のスコープです。</span><span class="sxs-lookup"><span data-stu-id="91597-138">The scope of the search.</span></span> <span data-ttu-id="91597-139">可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。</span><span class="sxs-lookup"><span data-stu-id="91597-139">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="91597-140">たとえば、管理者は別の組織をその「パートナー」に設定できます。</span><span class="sxs-lookup"><span data-stu-id="91597-140">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="91597-141">スコープは、管理者が特定のメール ヒントが特定のスコープにアクセスできるようにしたい場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="91597-141">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="91597-142">メッセージが組織から送信されても支障がないことを送信者に伝えたり、言葉遣いや文調、内容について正しい判断を下せるよう支援するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="91597-142">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="91597-143">RecipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="91597-143">RecipientSuggestions</span></span> | <span data-ttu-id="91597-144">[recipient](../resources/recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91597-144">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="91597-145">同じメッセージに表示される前のコンテキストに基づいて提案される受信者。</span><span class="sxs-lookup"><span data-stu-id="91597-145">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="91597-146">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="91597-146">TotalMemberCount</span></span> | <span data-ttu-id="91597-147">Int32</span><span class="sxs-lookup"><span data-stu-id="91597-147">Int32</span></span> | <span data-ttu-id="91597-148">受信者が配布リストの場合はメンバー数です。</span><span class="sxs-lookup"><span data-stu-id="91597-148">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91597-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91597-149">JSON representation</span></span>

<span data-ttu-id="91597-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91597-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->