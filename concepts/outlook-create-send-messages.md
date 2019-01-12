---
title: メッセージの作成、送信、処理の自動化
description: Microsoft Graph では、メールは message リソースで表されます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 160db6aae079d90f1ce20640429181cdbe6a4da5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927612"
---
# <a name="automate-creating-sending-and-processing-messages"></a><span data-ttu-id="6565c-103">メッセージの作成、送信、処理の自動化</span><span class="sxs-lookup"><span data-stu-id="6565c-103">Automate creating, sending, and processing messages</span></span>

<span data-ttu-id="6565c-104">Microsoft Graph では、メールは [message](/graph/api/resources/message?view=graph-rest-1.0) リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="6565c-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="6565c-105">既定で、メッセージは **id** プロパティの一意のエントリ ID で識別されます。</span><span class="sxs-lookup"><span data-stu-id="6565c-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="6565c-106">ストア プロバイダーは、メッセージが最初に作成されて、下書きとして保存されるか送信されるときに、そのメッセージにエントリ ID を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="6565c-106">When a message is initially created and saved as a draft or sent, the store provider assigns the message an entry ID.</span></span> <span data-ttu-id="6565c-107">既定でこの ID は、メッセージを別のフォルダー、ストア、.PST ファイルにコピーしたり移動したりすると、変更されます。</span><span class="sxs-lookup"><span data-stu-id="6565c-107">By default, that ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span> <span data-ttu-id="6565c-108">今後の処理のために、メッセージは現在の ID で参照されます。</span><span class="sxs-lookup"><span data-stu-id="6565c-108">You reference the message by its current ID for further processing.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="6565c-109">メールの作成と送信</span><span class="sxs-lookup"><span data-stu-id="6565c-109">Creating and sending mail</span></span>

<span data-ttu-id="6565c-110">Outlook では、同じ [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) アクションでメールを作成および送信できます。また、下書きを[作成](/graph/api/user-post-messages?view=graph-rest-1.0)してから[コンテンツを追加](/graph/api/message-update?view=graph-rest-1.0)し、その下書きを[送信](/graph/api/message-send?view=graph-rest-1.0)することもできます。</span><span class="sxs-lookup"><span data-stu-id="6565c-110">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="6565c-111">同様に、メールに返信する場合も、同じアクションで返信を送信できます ([返信](/graph/api/message-reply?view=graph-rest-1.0)、[全員に返信](/graph/api/message-replyall?view=graph-rest-1.0)、または[転送](/graph/api/message-forward?view=graph-rest-1.0))。</span><span class="sxs-lookup"><span data-stu-id="6565c-111">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="6565c-112">また、返信の下書きを作成 ([返信](/graph/api/message-createreply?view=graph-rest-1.0)、[全員に返信](/graph/api/message-createreplyall?view=graph-rest-1.0)、または[転送](/graph/api/message-createforward?view=graph-rest-1.0)) してから[コンテンツを追加](/graph/api/message-update?view=graph-rest-1.0)し、その下書きを後で[送信](/graph/api/message-send?view=graph-rest-1.0)することもできます。</span><span class="sxs-lookup"><span data-stu-id="6565c-112">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="6565c-113">下書きと送信済みメッセージをプログラムで区別するには、**isDraft** プロパティを確認します。</span><span class="sxs-lookup"><span data-stu-id="6565c-113">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="6565c-114">既定では、下書きメッセージは `Drafts` フォルダーに保存され、送信済みメッセージは `Sent Items` フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="6565c-114">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="6565c-115">利便性のため、Drafts フォルダーと SentItems フォルダーを、それぞれに対応する[わかりやすいフォルダー名](/graph/api/resources/mailfolder?view=graph-rest-1.0)で指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="6565c-115">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span> 

### <a name="setting-the-from-and-sender-properties"></a><span data-ttu-id="6565c-116">from プロパティと sender プロパティの設定</span><span class="sxs-lookup"><span data-stu-id="6565c-116">Setting the from and sender properties</span></span>

<span data-ttu-id="6565c-117">メッセージの作成中、Outlook はたいてい **from** プロパティと **sender** プロパティを同じサインイン ユーザーに設定しています。</span><span class="sxs-lookup"><span data-stu-id="6565c-117">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="6565c-118">次のシナリオでは、これらのプロパティを更新できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-118">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="6565c-p105">**From** プロパティは、Exchange 管理者がメールボックスの **SendAs** 権限を他のユーザーに割り当てた場合には変更が可能です。管理者は、Azure ポータルでメールボックス所有者の **メールボックスのアクセス許可** を選択するか、Exchange 管理センターまたは Windows PowerShell Add-ADPermission コマンドレットを使用してこれを行えます。その後、プログラムを使用して、**From** プロパティを、対象メールボックスの **SendAs** 権限を持ついずれかのユーザーに自動的に設定できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="6565c-122">**sender** プロパティは、メールボックス所有者が 1 人以上のユーザーにそのメールボックスからメッセージを送信する権限を委任すると、変更できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-122">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="6565c-123">メールボックス所有者は、Outlook で委任できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-123">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="6565c-124">代理人がメールボックス所有者に代わってメッセージを送信する場合、Outlook は **sender** プロパティを代理人のアカウントに設定し、**from** プロパティはメールボックス所有者のままになります。</span><span class="sxs-lookup"><span data-stu-id="6565c-124">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="6565c-125">プログラムを使用して、対象メールボックスの委任アクセス許可を取得したユーザーに **sender** プロパティを設定することができます。</span><span class="sxs-lookup"><span data-stu-id="6565c-125">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="6565c-126">MailTips を使用して受信者の状態を確認し、時間を節約する (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6565c-126">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="6565c-127">[MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) を使用すると、メールを送信する前にスマートに意思決定できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-127">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="6565c-128">MailTips を使用すると、受信者のメールボックスが特定の送信者のみに制限されているかどうかや、その受信者にメールを送信するには承認が必要かなどの情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-128">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>


## <a name="reading-messages-with-control-over-the-body-format-returned"></a><span data-ttu-id="6565c-129">返される本文の形式を制御したメッセージの読み取り</span><span class="sxs-lookup"><span data-stu-id="6565c-129">Reading messages with control over the body format returned</span></span>

<span data-ttu-id="6565c-130">ID を参照してメールボックス内の[メッセージを読み取る](/graph/api/message-get?view=graph-rest-1.0)ことができます。</span><span class="sxs-lookup"><span data-stu-id="6565c-130">You can [read a message](/graph/api/message-get?view=graph-rest-1.0) in a mailbox by referencing its ID:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

または、特定のフォルダー内の[メッセージを取得する](/graph/api/user-list-messages?view=graph-rest-1.0)ことができます。 <span data-ttu-id="6565c-132">たとえば、サインインしたユーザーの下書きフォルダーにあるメッセージを読み取るには、以下を行います。</span><span class="sxs-lookup"><span data-stu-id="6565c-132">For example, to read messages in the signed-in user's Drafts folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

<span data-ttu-id="6565c-133">Outlook メッセージの本文には、HTML 形式かテキスト形式を使用できます。GET 応答で返される既定のメッセージ本文の種類は HTML 形式です。</span><span class="sxs-lookup"><span data-stu-id="6565c-133">The body of an Outlook message can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="6565c-134">メッセージを取得する際に、次の要求ヘッダーで、**body** プロパティと **uniqueBody** プロパティがテキスト形式で返されるように指定できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-134">When getting a message, you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="6565c-135">HTML 形式でメッセージ本文を取得するには、次のヘッダーを指定するか、単にこのヘッダーをスキップします。</span><span class="sxs-lookup"><span data-stu-id="6565c-135">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="6565c-136">いずれかのヘッダーを指定した場合、成功応答には対応する `Preference-Applied` ヘッダーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6565c-136">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="6565c-137">テキスト形式要求の場合: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="6565c-137">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="6565c-138">HTML 形式要求の場合: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="6565c-138">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="6565c-139">本文が HTML の場合、既定では、Outlook は **body** プロパティに埋め込まれている安全でない可能性のある HTML (JavaScript など) を削除してから、本文の内容を REST 応答で返します。</span><span class="sxs-lookup"><span data-stu-id="6565c-139">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="6565c-140">元の HTML コンテンツ全体を取得するには、次の HTTP 要求ヘッダーを含めます。</span><span class="sxs-lookup"><span data-stu-id="6565c-140">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="6565c-141">@ ソーシャル ジェスチャとの統合 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6565c-141">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="6565c-142">@ メンションとは、それらがメッセージに含まれている場合にユーザーに警告する通知のことです。</span><span class="sxs-lookup"><span data-stu-id="6565c-142">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="6565c-143">[mention](/graph/api/resources/mention?view=graph-rest-beta) リソースを使用すると、メールに含まれる一般的なオンライン ソーシャル ジェスチャである @ プレフィックスを、アプリで設定および取得できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-143">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="6565c-144">次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="6565c-144">You can:</span></span>

- <span data-ttu-id="6565c-145">[メッセージを作成](/graph/api/user-post-messages?view=graph-rest-beta#request-2)する際に @ メンションを作成する</span><span class="sxs-lookup"><span data-stu-id="6565c-145">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="6565c-146">ユーザーのメールボックス内にある、そのユーザーの @ メンションを含むすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="6565c-146">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="6565c-147">メッセージ内の @ メンションすべてを取得する</span><span class="sxs-lookup"><span data-stu-id="6565c-147">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="6565c-148">その他の共有機能</span><span class="sxs-lookup"><span data-stu-id="6565c-148">Other shared capabilities</span></span>

<span data-ttu-id="6565c-149">Microsoft Graph エンティティ間で共有されている次の一般的な機能を活用します。</span><span class="sxs-lookup"><span data-stu-id="6565c-149">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="6565c-150">メッセージの作成や更新など、1 つ以上の種類の変更が発生した場合の、メッセージの[変更通知](/graph/api/resources/webhooks?view=graph-rest-1.0)を受信登録します。</span><span class="sxs-lookup"><span data-stu-id="6565c-150">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="6565c-151">[フォルダー内のメッセージへの増分の変更を追跡](delta-query-messages.md)します。</span><span class="sxs-lookup"><span data-stu-id="6565c-151">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="6565c-152">[オープン拡張機能](extensibility-overview.md#open-extensions)や[スキーマ拡張機能](extensibility-overview.md#schema-extensions)を作成して、メッセージ インスタンスにカスタム データを追加します。</span><span class="sxs-lookup"><span data-stu-id="6565c-152">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="6565c-153">Outlook MAPI プロパティが Microsoft Graph API メタデータでまだ公開されていない場合は、メッセージ インスタンスで[拡張プロパティ](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0)を作成して、それらのプロパティのカスタム データを保存します。</span><span class="sxs-lookup"><span data-stu-id="6565c-153">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6565c-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="6565c-154">Next steps</span></span>

<span data-ttu-id="6565c-155">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="6565c-155">Find out more about:</span></span>

- [<span data-ttu-id="6565c-156">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="6565c-156">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- [<span data-ttu-id="6565c-157">Outlook リソースの不変 ID の取得 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6565c-157">Get immutable identifiers for Outlook resources (preview)</span></span>](outlook-immutable-id.md)
- <span data-ttu-id="6565c-158">Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="6565c-158">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
