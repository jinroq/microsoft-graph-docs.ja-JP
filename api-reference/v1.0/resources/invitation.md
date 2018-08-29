# <a name="invitation-manager"></a><span data-ttu-id="0263e-101">招待マネージャー</span><span class="sxs-lookup"><span data-stu-id="0263e-101">invitation manager</span></span>

<span data-ttu-id="0263e-102">招待マネージャーを使用して、組織に外部ユーザーを追加するための招待状を作成します。</span><span class="sxs-lookup"><span data-stu-id="0263e-102">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="0263e-103">招待処理では、次のフローが使用されます。</span><span class="sxs-lookup"><span data-stu-id="0263e-103">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="0263e-104">招待状が作成されます。</span><span class="sxs-lookup"><span data-stu-id="0263e-104">An invitation is created</span></span>
* <span data-ttu-id="0263e-105">招待状が招待ユーザーに送信されます (招待状リンクを含む)。</span><span class="sxs-lookup"><span data-stu-id="0263e-105">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="0263e-106">招待ユーザーが招待状リンクをクリックしてサインインし、招待状を引き換え、招待ユーザーを表すユーザー エンティティの作成が完了します。</span><span class="sxs-lookup"><span data-stu-id="0263e-106">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="0263e-107">引き換えが完了した後、特定のページにユーザーがリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="0263e-107">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="0263e-p101">招待状を作成すると、応答で引き換え URL が返されます (*inviteRedeemUrl*)。招待状作成 API では、*sendInvitationMessage* を true に設定することにより、引き換え URL を含むメールが自動的に招待ユーザーに送信されます。招待ユーザーに送信されるメッセージをカスタマイズすることもできます。代わりに、他の手段で引き換え URL を送信したい場合は、*sendInvitationMessage* を false に設定し、応答からの引き換え URL を使用して、独自の通信を作成することもできます。現在、引き換え処理を実行するための API はありません。招待ユーザーは、上記手順の通信で送信された *inviteRedeemUrl* リンクをクリックして、対話型引き換え処理をブラウザーで行う必要があります。完了すると、招待ユーザーは、組織における外部ユーザーになります。</span><span class="sxs-lookup"><span data-stu-id="0263e-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="0263e-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="0263e-115">Methods</span></span>
| <span data-ttu-id="0263e-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="0263e-116">Method</span></span>       | <span data-ttu-id="0263e-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0263e-117">Return Type</span></span>  |<span data-ttu-id="0263e-118">説明</span><span class="sxs-lookup"><span data-stu-id="0263e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0263e-119">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="0263e-119">Create invitation</span></span>](../api/invitation_post.md) | <span data-ttu-id="0263e-120">invitation</span><span class="sxs-lookup"><span data-stu-id="0263e-120">invitation</span></span> | <span data-ttu-id="0263e-121">招待状オブジェクトのプロパティと関係を書き込みます。</span><span class="sxs-lookup"><span data-stu-id="0263e-121">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0263e-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0263e-122">Properties</span></span>
| <span data-ttu-id="0263e-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0263e-123">Property</span></span>     | <span data-ttu-id="0263e-124">タイプ</span><span class="sxs-lookup"><span data-stu-id="0263e-124">Type</span></span>   |<span data-ttu-id="0263e-125">説明</span><span class="sxs-lookup"><span data-stu-id="0263e-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0263e-126">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="0263e-126">invitedUserDisplayName</span></span>|<span data-ttu-id="0263e-127">String</span><span class="sxs-lookup"><span data-stu-id="0263e-127">String</span></span>|<span data-ttu-id="0263e-128">招待されるユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="0263e-128">The display name of the user being invited.</span></span>|
|<span data-ttu-id="0263e-129">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0263e-129">invitedUserEmailAddress</span></span>|<span data-ttu-id="0263e-130">String</span><span class="sxs-lookup"><span data-stu-id="0263e-130">String</span></span>|<span data-ttu-id="0263e-p102">招待されるユーザーのメール アドレス。必須。</span><span class="sxs-lookup"><span data-stu-id="0263e-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="0263e-133">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0263e-133">invitedUserMessageInfo</span></span>|[<span data-ttu-id="0263e-134">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0263e-134">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="0263e-135">メッセージ テキスト、言語、および cc 受信者リストのカスタマイズなど、招待ユーザーに送信されるメッセージの追加構成。</span><span class="sxs-lookup"><span data-stu-id="0263e-135">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="0263e-136">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="0263e-136">sendInvitationMessage</span></span>|<span data-ttu-id="0263e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0263e-137">Boolean</span></span>|<span data-ttu-id="0263e-p103">招待されるユーザーにメールを送信するかどうかを示します。既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="0263e-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="0263e-140">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="0263e-140">inviteRedirectUrl</span></span>|<span data-ttu-id="0263e-141">String</span><span class="sxs-lookup"><span data-stu-id="0263e-141">String</span></span>|<span data-ttu-id="0263e-p104">招待状が引き換えられるとにユーザーがリダイレクトされる URL。必須。</span><span class="sxs-lookup"><span data-stu-id="0263e-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="0263e-144">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="0263e-144">inviteRedeemUrl</span></span>|<span data-ttu-id="0263e-145">String</span><span class="sxs-lookup"><span data-stu-id="0263e-145">String</span></span>|<span data-ttu-id="0263e-p105">ユーザーが招待状の引き換えに使用できる URL。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0263e-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="0263e-148">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="0263e-148">invitedUserType</span></span>|<span data-ttu-id="0263e-149">String</span><span class="sxs-lookup"><span data-stu-id="0263e-149">String</span></span>|<span data-ttu-id="0263e-150">招待されるユーザーの userType。</span><span class="sxs-lookup"><span data-stu-id="0263e-150">The userType of the user being invited.</span></span> <span data-ttu-id="0263e-151">既定では Guest です。</span><span class="sxs-lookup"><span data-stu-id="0263e-151">By default, this is Guest.</span></span> <span data-ttu-id="0263e-152">会社の管理者の場合は、Member として招待できます。</span><span class="sxs-lookup"><span data-stu-id="0263e-152">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="0263e-153">status</span><span class="sxs-lookup"><span data-stu-id="0263e-153">status</span></span>|<span data-ttu-id="0263e-154">String</span><span class="sxs-lookup"><span data-stu-id="0263e-154">String</span></span>|<span data-ttu-id="0263e-p107">招待の状態。可能な値:PendingAcceptance、Completed、InProgress、および Error</span><span class="sxs-lookup"><span data-stu-id="0263e-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="0263e-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0263e-157">Relationships</span></span>
| <span data-ttu-id="0263e-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0263e-158">Relationship</span></span> | <span data-ttu-id="0263e-159">型</span><span class="sxs-lookup"><span data-stu-id="0263e-159">Type</span></span>   |<span data-ttu-id="0263e-160">説明</span><span class="sxs-lookup"><span data-stu-id="0263e-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0263e-161">invitedUser</span><span class="sxs-lookup"><span data-stu-id="0263e-161">invitedUser</span></span>|[<span data-ttu-id="0263e-162">User</span><span class="sxs-lookup"><span data-stu-id="0263e-162">User</span></span>](user.md)|<span data-ttu-id="0263e-p108">招待状作成の一環として作成されたユーザー。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0263e-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0263e-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0263e-165">JSON representation</span></span>
<span data-ttu-id="0263e-166">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0263e-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
