# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="ad064-101">Microsoft Graph API を使用して変更通知を取得するには</span><span class="sxs-lookup"><span data-stu-id="ad064-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="ad064-102">Microsoft Graph の REST API は、Webhook メカニズムを使用して、クライアントに通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="ad064-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="ad064-103">クライアントは、通知を受信するために自身の URL を構成する Web サービスです。</span><span class="sxs-lookup"><span data-stu-id="ad064-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="ad064-104">クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="ad064-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="ad064-105">受信通知を購読・処理する方法の詳細については、「[ユーザー データの変更に関する通知の設定](../../../concepts/webhooks.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad064-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="ad064-106">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="ad064-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="ad064-107">メッセージ</span><span class="sxs-lookup"><span data-stu-id="ad064-107">Messages</span></span>
- <span data-ttu-id="ad064-108">イベント</span><span class="sxs-lookup"><span data-stu-id="ad064-108">Events</span></span>
- <span data-ttu-id="ad064-109">連絡先</span><span class="sxs-lookup"><span data-stu-id="ad064-109">Contacts</span></span>
- <span data-ttu-id="ad064-110">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ad064-110">Users</span></span>
- <span data-ttu-id="ad064-111">グループ</span><span class="sxs-lookup"><span data-stu-id="ad064-111">Groups</span></span>
- <span data-ttu-id="ad064-112">グループ会話</span><span class="sxs-lookup"><span data-stu-id="ad064-112">Group conversations</span></span>
- <span data-ttu-id="ad064-113">SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="ad064-113">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="ad064-114">ユーザーの個人用 OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="ad064-114">User's personal OneDrive folders</span></span>

## <a name="permissions"></a><span data-ttu-id="ad064-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad064-115">Permissions</span></span>

<span data-ttu-id="ad064-p102">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ad064-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="ad064-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad064-120">Permission type</span></span>                        | <span data-ttu-id="ad064-121">v1.0 でサポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="ad064-121">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="ad064-122">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="ad064-122">Delegated - work or school account</span></span>     | <span data-ttu-id="ad064-123">[連絡先][]、[スレッド][]、[ドライブ][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="ad064-123">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="ad064-124">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="ad064-124">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="ad064-125">なし</span><span class="sxs-lookup"><span data-stu-id="ad064-125">None</span></span>                                                             |
| <span data-ttu-id="ad064-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad064-126">Application</span></span>                            | <span data-ttu-id="ad064-127">[連絡先][]、[スレッド][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="ad064-127">[contact][], [conversation][], [event][], [message][]</span></span>            |

## <a name="see-also"></a><span data-ttu-id="ad064-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="ad064-128">See also</span></span>

- [<span data-ttu-id="ad064-129">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="ad064-129">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="ad064-130">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="ad064-130">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="ad064-131">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="ad064-131">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="ad064-132">サブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="ad064-132">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="ad064-133">サブスクリプションを削除する</span><span class="sxs-lookup"><span data-stu-id="ad064-133">Delete subscription</span></span>](../api/subscription_delete.md)

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
