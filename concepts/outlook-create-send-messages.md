# <a name="create-and-send-outlook-messages"></a><span data-ttu-id="645e0-101">Outlook メッセージを作成して送信する</span><span class="sxs-lookup"><span data-stu-id="645e0-101">Create and send Outlook messages</span></span>

<span data-ttu-id="645e0-102">Microsoft Graph では、メールは [message](../api-reference/v1.0/resources/message.md) リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="645e0-102">Emails are represented by the [message](../api-reference/v1.0/resources/message.md) resource in Microsoft Graph.</span></span>

<span data-ttu-id="645e0-103">既定で、メッセージは **id** プロパティの一意のエントリ ID で識別されます。</span><span class="sxs-lookup"><span data-stu-id="645e0-103">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="645e0-104">ストア プロバイダーは、メッセージが最初に下書きとして保存されるか送信されるときに、メッセージにエントリ ID を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="645e0-104">A store provider assigns a message an entry ID when the message is initially saved as a draft or sent.</span></span> <span data-ttu-id="645e0-105">この ID は、メッセージを別のフォルダー、ストア、または .PST ファイルにコピーしたり移動したりすると、変更されます。</span><span class="sxs-lookup"><span data-stu-id="645e0-105">That ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="645e0-106">メールの作成と送信</span><span class="sxs-lookup"><span data-stu-id="645e0-106">Creating and sending mail</span></span>

<span data-ttu-id="645e0-107">Outlook では、同じ [sendMail](../api-reference/v1.0/api/user_sendmail.md) アクションでメールを作成および送信できます。また、下書きを[作成](../api-reference/v1.0/api/user_post_messages.md)してから[コンテンツを追加](../api-reference/v1.0/api/message_update.md)し、その下書きを[送信](../api-reference/v1.0/api/message_send.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="645e0-107">In Outlook, you can create and send an email in the same [sendMail](../api-reference/v1.0/api/user_sendmail.md) action, or you can [create](../api-reference/v1.0/api/user_post_messages.md) a draft, subsequently [add content](../api-reference/v1.0/api/message_update.md) and [send](../api-reference/v1.0/api/message_send.md) the draft.</span></span>

<span data-ttu-id="645e0-108">同様に、メールに返信する場合も、同じアクションで返信を送信できます ([返信](../api-reference/v1.0/api/message_reply.md)、[全員に返信](../api-reference/v1.0/api//message_replyall.md)、または[転送](../api-reference/v1.0/api/message_forward.md))。</span><span class="sxs-lookup"><span data-stu-id="645e0-108">Similarly, when responding to an email, you can create and send the response in the same action ([reply](../api-reference/v1.0/api/message_reply.md), [reply-all](../api-reference/v1.0/api//message_replyall.md), or [forward](../api-reference/v1.0/api/message_forward.md)).</span></span> <span data-ttu-id="645e0-109">また、返信の下書きを作成 ([返信](../api-reference/v1.0/api/message_createreply.md)、[全員に返信](../api-reference/v1.0/api//message_createreplyall.md)、または[転送](../api-reference/v1.0/api/message_createforward.md)) してから[コンテンツを追加](../api-reference/v1.0/api/message_update.md)し、その下書きを後で[送信](../api-reference/v1.0/api/message_send.md)することもできます。</span><span class="sxs-lookup"><span data-stu-id="645e0-109">Or, you can create a draft for the response ([reply](../api-reference/v1.0/api/message_createreply.md), [reply-all](../api-reference/v1.0/api//message_createreplyall.md), or [forward](../api-reference/v1.0/api/message_createforward.md)), [add content](../api-reference/v1.0/api/message_update.md), and then [send](../api-reference/v1.0/api/message_send.md) the draft at a later time.</span></span>

<span data-ttu-id="645e0-110">下書きと送信済みメッセージをプログラムで区別するには、**isDraft** プロパティを確認します。</span><span class="sxs-lookup"><span data-stu-id="645e0-110">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="645e0-111">既定では、下書きメッセージは `Drafts` フォルダーに保存され、送信済みメッセージは `Sent Items` フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="645e0-111">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="645e0-112">利便性のため、Drafts フォルダーと SentItems フォルダーを、それぞれに対応する[わかりやすいフォルダー名](../api-reference/v1.0/resources/mailfolder.md)で指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="645e0-112">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](../api-reference/v1.0/resources/mailfolder.md).</span></span> <span data-ttu-id="645e0-113">たとえば、次のようにして Drafts フォルダー内の[メッセージを取得](../api-reference/v1.0/api/user_list_messages.md)できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-113">For example, you can do the following to [get the messages](../api-reference/v1.0/api/user_list_messages.md) in the Drafts folder:</span></span>

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a><span data-ttu-id="645e0-114">本文の形式と悪意のあるスクリプト</span><span class="sxs-lookup"><span data-stu-id="645e0-114">Body format and malicious script</span></span>

<!-- Remove the following 2 sections from the message.md topics
-->

<span data-ttu-id="645e0-115">メッセージ本文には、HTML 形式かテキスト形式を使用できます。GET 応答で返される既定のメッセージ本文の種類は HTML 形式です。</span><span class="sxs-lookup"><span data-stu-id="645e0-115">The message body can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="645e0-116">[メッセージを取得](../api-reference/v1.0/api/message_get.md)する際に、次の要求ヘッダーで、**body** プロパティと **uniqueBody** プロパティがテキスト形式で返されるように指定できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-116">When [getting a message](../api-reference/v1.0/api/message_get.md), you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="645e0-117">HTML 形式でメッセージ本文を取得するには、次のヘッダーを指定するか、単にこのヘッダーをスキップします。</span><span class="sxs-lookup"><span data-stu-id="645e0-117">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="645e0-118">いずれかのヘッダーを指定した場合、成功応答には対応する `Preference-Applied` ヘッダーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="645e0-118">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="645e0-119">テキスト形式要求の場合: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="645e0-119">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="645e0-120">HTML 形式要求の場合: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="645e0-120">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="645e0-121">本文が HTML の場合、既定では、Outlook は **body** プロパティに埋め込まれている安全でない可能性のある HTML (JavaScript など) を削除してから、本文の内容を REST 応答で返します。</span><span class="sxs-lookup"><span data-stu-id="645e0-121">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="645e0-122">元の HTML コンテンツ全体を取得するには、次の HTTP 要求ヘッダーを含めます。</span><span class="sxs-lookup"><span data-stu-id="645e0-122">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a><span data-ttu-id="645e0-123">from プロパティと sender プロパティの区別</span><span class="sxs-lookup"><span data-stu-id="645e0-123">Differentiating the from and sender properties</span></span>

<span data-ttu-id="645e0-124">メッセージの作成中、Outlook はたいてい **from** プロパティと **sender** プロパティを同じサインイン ユーザーに設定しています。</span><span class="sxs-lookup"><span data-stu-id="645e0-124">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="645e0-125">次のシナリオでは、これらのプロパティを更新できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-125">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="645e0-p105">**From** プロパティは、Exchange 管理者がメールボックスの **SendAs** 権限を他のユーザーに割り当てた場合には変更が可能です。管理者は、Azure ポータルでメールボックス所有者の **メールボックスのアクセス許可** を選択するか、Exchange 管理センターまたは Windows PowerShell Add-ADPermission コマンドレットを使用してこれを行えます。その後、プログラムを使用して、**From** プロパティを、対象メールボックスの **SendAs** 権限を持ついずれかのユーザーに自動的に設定できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="645e0-129">**sender** プロパティは、メールボックス所有者が 1 人以上のユーザーにそのメールボックスからメッセージを送信する権限を委任すると、変更できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-129">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="645e0-130">メールボックス所有者は、Outlook で委任できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-130">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="645e0-131">代理人がメールボックス所有者に代わってメッセージを送信する場合、Outlook は **sender** プロパティを代理人のアカウントに設定し、**from** プロパティはメールボックス所有者のままになります。</span><span class="sxs-lookup"><span data-stu-id="645e0-131">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="645e0-132">プログラムを使用して、対象メールボックスの委任アクセス許可を取得したユーザーに **sender** プロパティを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="645e0-132">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="645e0-133">MailTips を使用して受信者の状態を確認し、時間を節約する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="645e0-133">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="645e0-134">[MailTips](../api-reference/beta/resources/mailtips.md) を使用すると、メールを送信する前にスマートに意思決定できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-134">Use [MailTips](../api-reference/beta/resources/mailtips.md) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="645e0-135">MailTips を使用すると、受信者のメールボックスが特定の送信者のみに制限されているかどうかや、その受信者にメールを送信するには承認が必要かなどの情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-135">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="645e0-136">@ ソーシャル ジェスチャとの統合 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="645e0-136">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="645e0-137">@ メンションとは、それらがメッセージに含まれている場合にユーザーに警告する通知のことです。</span><span class="sxs-lookup"><span data-stu-id="645e0-137">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="645e0-138">[mention](../api-reference/beta/resources/mention.md) リソースを使用すると、メールに含まれる一般的なオンライン ソーシャル ジェスチャである @ プレフィックスを、アプリで設定および取得できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-138">The [mention](../api-reference/beta/resources/mention.md) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="645e0-139">次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="645e0-139">You can:</span></span>

- <span data-ttu-id="645e0-140">[メッセージを作成](../api-reference/beta/api/user_post_messages.md#request-2)する際に @ メンションを作成する</span><span class="sxs-lookup"><span data-stu-id="645e0-140">Create @-mentions when [creating a message](../api-reference/beta/api/user_post_messages.md#request-2)</span></span>
- [<span data-ttu-id="645e0-141">ユーザーのメールボックス内にある、そのユーザーの @ メンションを含むすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="645e0-141">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](../api-reference/beta/api/user_list_messages.md#request-2)
- [<span data-ttu-id="645e0-142">メッセージ内の @ メンションすべてを取得する</span><span class="sxs-lookup"><span data-stu-id="645e0-142">Get all the @-mention is a message</span></span>](../api-reference/beta/api/message_get.md#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="645e0-143">その他の共有機能</span><span class="sxs-lookup"><span data-stu-id="645e0-143">Other shared capabilities</span></span>

<span data-ttu-id="645e0-144">Microsoft Graph エンティティ間で共有されている次の一般的な機能を活用します。</span><span class="sxs-lookup"><span data-stu-id="645e0-144">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="645e0-145">メッセージの作成や更新など、1 つ以上の種類の変更が発生した場合の、メッセージの[変更通知](../api-reference/v1.0/resources/webhooks.md)を受信登録します。</span><span class="sxs-lookup"><span data-stu-id="645e0-145">Subscribe to [change notifications](../api-reference/v1.0/resources/webhooks.md) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="645e0-146">[フォルダー内のメッセージへの増分の変更を追跡](delta_query_messages.md)します。</span><span class="sxs-lookup"><span data-stu-id="645e0-146">[Track these incremental changes to messages in a folder](delta_query_messages.md).</span></span>
- <span data-ttu-id="645e0-147">[オープン拡張機能](extensibility_overview.md#open-extensions)や[スキーマ拡張機能](extensibility_overview.md#schema-extensions)を作成して、メッセージ インスタンスにカスタム データを追加します。</span><span class="sxs-lookup"><span data-stu-id="645e0-147">Create [open extensions](extensibility_overview.md#open-extensions) or [schema extensions](extensibility_overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="645e0-148">Outlook MAPI プロパティが Microsoft Graph API メタデータでまだ公開されていない場合は、メッセージ インスタンスで[拡張プロパティ](../api-reference/v1.0/resources/extended-properties-overview.md)を作成して、それらのプロパティのカスタム データを保存します。</span><span class="sxs-lookup"><span data-stu-id="645e0-148">Create [extended properties](../api-reference/v1.0/resources/extended-properties-overview.md) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="645e0-149">次の手順</span><span class="sxs-lookup"><span data-stu-id="645e0-149">Next steps</span></span>

<span data-ttu-id="645e0-150">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="645e0-150">Find out more about:</span></span>

- [<span data-ttu-id="645e0-151">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="645e0-151">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="645e0-152">Microsoft Graph v1.0 の[メール API](../api-reference/v1.0/resources/mail_api_overview.md) とその[用途](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)</span><span class="sxs-lookup"><span data-stu-id="645e0-152">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-create-send-messages.md:
        BookmarkSkippedDocFileNotFound: Link '[creating a message](../api-reference/beta/api/user_post_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the messages in a user's mailbox that contain an @-mention of the user](../api-reference/beta/api/user_list_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the @-mention is a message](../api-reference/beta/api/message_get.md#request-2)'."
  ]
}-->
