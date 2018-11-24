# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="cc6c7-101">変更通知を使用して Microsoft グラフ API を取得するには</span><span class="sxs-lookup"><span data-stu-id="cc6c7-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="cc6c7-102">Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="cc6c7-103">クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="cc6c7-104">クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="cc6c7-105">詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](../../../concepts/webhooks.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="cc6c7-106">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="cc6c7-107">メッセージ</span><span class="sxs-lookup"><span data-stu-id="cc6c7-107">Messages</span></span>
- <span data-ttu-id="cc6c7-108">イベント</span><span class="sxs-lookup"><span data-stu-id="cc6c7-108">Events</span></span>
- <span data-ttu-id="cc6c7-109">連絡先</span><span class="sxs-lookup"><span data-stu-id="cc6c7-109">Contacts</span></span>
- <span data-ttu-id="cc6c7-110">ユーザー</span><span class="sxs-lookup"><span data-stu-id="cc6c7-110">Users</span></span>
- <span data-ttu-id="cc6c7-111">グループ</span><span class="sxs-lookup"><span data-stu-id="cc6c7-111">Groups</span></span>
- <span data-ttu-id="cc6c7-112">グループ会話</span><span class="sxs-lookup"><span data-stu-id="cc6c7-112">Group conversations</span></span>
- <span data-ttu-id="cc6c7-113">SharePoint サイトに関連付けられているドライブを含む、OneDrive で共有されているコンテンツ</span><span class="sxs-lookup"><span data-stu-id="cc6c7-113">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="cc6c7-114">ユーザーの個人用の OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="cc6c7-114">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="cc6c7-115">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="cc6c7-115">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="cc6c7-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc6c7-116">Permissions</span></span>

<span data-ttu-id="cc6c7-p102">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="cc6c7-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="cc6c7-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc6c7-121">Permission type</span></span>                        | <span data-ttu-id="cc6c7-122">v1.0 でサポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="cc6c7-122">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="cc6c7-123">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="cc6c7-123">Delegated - work or school account</span></span>     | <span data-ttu-id="cc6c7-124">[お問い合わせください][]、[会話][]、[ドライブ][]、[イベント][]、[メッセージ][]、[警告][]</span><span class="sxs-lookup"><span data-stu-id="cc6c7-124">[contact][], [conversation][], [drive][], [event][], [message][], [alert][]</span></span> |
| <span data-ttu-id="cc6c7-125">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="cc6c7-125">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="cc6c7-126">なし</span><span class="sxs-lookup"><span data-stu-id="cc6c7-126">None</span></span>                                                             |
| <span data-ttu-id="cc6c7-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc6c7-127">Application</span></span>                            | <span data-ttu-id="cc6c7-128">[お問い合わせください][]、[会話][]、[イベント][]、[メッセージ][]、[警告][]</span><span class="sxs-lookup"><span data-stu-id="cc6c7-128">[contact][], [conversation][], [event][], [message][], [alert][]</span></span>           |

## <a name="see-also"></a><span data-ttu-id="cc6c7-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc6c7-129">See also</span></span>

- [<span data-ttu-id="cc6c7-130">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="cc6c7-130">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="cc6c7-131">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="cc6c7-131">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="cc6c7-132">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="cc6c7-132">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="cc6c7-133">Update subscription</span><span class="sxs-lookup"><span data-stu-id="cc6c7-133">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="cc6c7-134">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="cc6c7-134">Delete subscription</span></span>](../api/subscription_delete.md)

[連絡先]: ./contact.md
[contact]: ./contact.md
[会話]: ./conversation.md
[conversation]: ./conversation.md
[ドライブ]: ./drive.md
[drive]: ./drive.md
[イベント]: ./event.md
[event]: ./event.md
[メッセージ]: ./message.md
[message]: ./message.md
[アラート]: ./alert.md
[alert]: ./alert.md