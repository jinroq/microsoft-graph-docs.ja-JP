# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="3feeb-101">Microsoft Graph の Webhooks での作業</span><span class="sxs-lookup"><span data-stu-id="3feeb-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="3feeb-p101">Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="3feeb-105">Microsoft Graph の REST API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="3feeb-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="3feeb-106">Messages</span><span class="sxs-lookup"><span data-stu-id="3feeb-106">Messages</span></span>
* <span data-ttu-id="3feeb-107">イベント</span><span class="sxs-lookup"><span data-stu-id="3feeb-107">Events</span></span>
* <span data-ttu-id="3feeb-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="3feeb-108">Contacts</span></span>
* <span data-ttu-id="3feeb-109">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3feeb-109">Users</span></span>
* <span data-ttu-id="3feeb-110">グループ</span><span class="sxs-lookup"><span data-stu-id="3feeb-110">Groups</span></span>
* <span data-ttu-id="3feeb-111">グループ会話</span><span class="sxs-lookup"><span data-stu-id="3feeb-111">Group conversations</span></span>
* <span data-ttu-id="3feeb-112">SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="3feeb-112">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="3feeb-113">ユーザーの個人用 OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="3feeb-113">User's personal OneDrive folders</span></span>

<span data-ttu-id="3feeb-114">たとえば、特定のフォルダーへサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="3feeb-114">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="3feeb-115">または、特定の ID: `users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="3feeb-115">Or a specific ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="3feeb-116">あるいは、最上位レベルのリソース: `me/messages`、`me/contacts`、`me/events`、`users`、または`groups`</span><span class="sxs-lookup"><span data-stu-id="3feeb-116">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`</span></span>

<span data-ttu-id="3feeb-117">Sharepoint/OneDrive for Business ドライブの場合: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="3feeb-117">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="3feeb-118">ユーザーの個人用 OneDrive の場合は次のようになります。`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="3feeb-118">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="3feeb-p102">Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。アプリはその後、そのビジネス ロジックに従ってアクションを実行します。たとえば、詳細データのフェッチ、キャッシュやビューの更新などです。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="3feeb-122">アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-122">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="3feeb-123">そうしない場合、新しいサブスクリプションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-123">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="3feeb-124">最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3feeb-124">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="3feeb-125">また、アプリはいつでも登録を解除して、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="3feeb-125">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="3feeb-p104">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api-reference/v1.0/api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api-reference/v1.0/api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="3feeb-130">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3feeb-130">Permission type</span></span>                        | <span data-ttu-id="3feeb-131">v1.0 でサポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="3feeb-131">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="3feeb-132">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="3feeb-132">Delegated - work or school account</span></span>     | <span data-ttu-id="3feeb-133">[連絡先][]、[スレッド][]、[ドライブ][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="3feeb-133">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="3feeb-134">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="3feeb-134">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="3feeb-135">なし</span><span class="sxs-lookup"><span data-stu-id="3feeb-135">None</span></span>                                                             |
| <span data-ttu-id="3feeb-136">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3feeb-136">Application</span></span>                            | <span data-ttu-id="3feeb-137">[連絡先][]、[スレッド][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="3feeb-137">[contact][], [conversation][], [event][], [message][]</span></span>            |


## <a name="code-samples"></a><span data-ttu-id="3feeb-138">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="3feeb-138">Code samples</span></span>

<span data-ttu-id="3feeb-139">GitHub では、次のコード サンプルを利用できます。</span><span class="sxs-lookup"><span data-stu-id="3feeb-139">The following code samples are available on GitHub.</span></span>

* [<span data-ttu-id="3feeb-140">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="3feeb-140">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="3feeb-141">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="3feeb-141">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a><span data-ttu-id="3feeb-142">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="3feeb-142">Creating a subscription</span></span>

<span data-ttu-id="3feeb-p105">リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="3feeb-145">クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-145">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="3feeb-146">Microsoft Graph が要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-146">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="3feeb-147">要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-147">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="3feeb-148">要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-148">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="3feeb-149">クライアントは、Microsoft Graph に検証トークンを返送します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-149">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="3feeb-150">クライアントは、対応するサブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-150">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

### <a name="notification-url-validation"></a><span data-ttu-id="3feeb-151">通知 URL の検証</span><span class="sxs-lookup"><span data-stu-id="3feeb-151">Notification URL validation</span></span>

<span data-ttu-id="3feeb-p106">Microsoft Graph は、サブスクリプションを作成する前にサブスクリプション要求の通知 URL を検証します。検証プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="3feeb-154">Microsoft Graph が通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-154">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. <span data-ttu-id="3feeb-155">クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-155">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="3feeb-156">200 (OK) 状態コード。</span><span class="sxs-lookup"><span data-stu-id="3feeb-156">A 200 (OK) status code.</span></span>
  * <span data-ttu-id="3feeb-157">コンテンツ タイプはテキスト/書式なしである必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-157">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="3feeb-158">本文には Microsoft Graph が提供した検証トークンを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-158">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="3feeb-159">クライアントは、応答を提供した後は検証トークンを破棄する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-159">The client should discard the validation token after providing it in the response.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="3feeb-160">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="3feeb-160">Subscription request example</span></span>

``` http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="3feeb-p107">プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。プロパティの定義と値については、「[サブスクリプション リソースの種類](../api-reference/v1.0/resources/subscription.md)」をご覧ください。`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="3feeb-164">処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](../api-reference/v1.0/resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-164">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="3feeb-165">Azure AD リソースの制限</span><span class="sxs-lookup"><span data-stu-id="3feeb-165">Azure AD Resource Limitations</span></span>

<span data-ttu-id="3feeb-166">Azure AD ベースのリソース (ユーザー、グループ) には一定の制限が適用され、超過するとエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-166">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

* <span data-ttu-id="3feeb-167">最大サブスクリプションのクォータ:</span><span class="sxs-lookup"><span data-stu-id="3feeb-167">Maximum subscription quotas:</span></span>

  * <span data-ttu-id="3feeb-168">アプリあたり: 合計 50,000 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="3feeb-168">Per App: 50,000 total subscriptions</span></span>
  * <span data-ttu-id="3feeb-169">テナントあたり: すべてのアプリで合計 35 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="3feeb-169">Per Tenant: 35 total subscriptions across all apps</span></span>
  * <span data-ttu-id="3feeb-170">アプリとテナントの組み合わせ: 合計 7 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="3feeb-170">Per App and Tenant combination: 7 total subscriptions</span></span>

* <span data-ttu-id="3feeb-171">Azure AD B2C テナントはサポートされていません</span><span class="sxs-lookup"><span data-stu-id="3feeb-171">Azure AD B2C tenants are not supported</span></span>

* <span data-ttu-id="3feeb-172">一般アカウント ユーザーはサポートされていません</span><span class="sxs-lookup"><span data-stu-id="3feeb-172">Consumer account Users not supported</span></span>

## <a name="renewing-a-subscription"></a><span data-ttu-id="3feeb-173">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="3feeb-173">Renewing a subscription</span></span>

<span data-ttu-id="3feeb-p108">クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。expirationDateTime プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

### <a name="subscription-renewal-example"></a><span data-ttu-id="3feeb-176">サブスクリプションの更新の例</span><span class="sxs-lookup"><span data-stu-id="3feeb-176">Subscription renewal example</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="3feeb-p109">処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](../api-reference/v1.0/resources/subscription.md) オブジェクトを返します。サブスクリプション オブジェクトには、新しい expirationDateTime の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

## <a name="deleting-a-subscription"></a><span data-ttu-id="3feeb-179">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="3feeb-179">Deleting a subscription</span></span>

<span data-ttu-id="3feeb-180">クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="3feeb-180">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="3feeb-181">処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-181">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="3feeb-182">通知</span><span class="sxs-lookup"><span data-stu-id="3feeb-182">Notifications</span></span>

<span data-ttu-id="3feeb-p110">クライアントはサブスクリプションを作成した後、通知の受信を開始します。Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。クライアントは、指定した変更の種類 (*created* など) に応じた通知のみを受信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="3feeb-186">通知のプロパティ</span><span class="sxs-lookup"><span data-stu-id="3feeb-186">Notification properties</span></span>

<span data-ttu-id="3feeb-187">通知オブジェクトには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-187">The notification object has the following properties:</span></span>

* <span data-ttu-id="3feeb-188">subscriptionId - この通知が属するサブスクリプションの ID。</span><span class="sxs-lookup"><span data-stu-id="3feeb-188">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="3feeb-189">subscriptionExpirationDateTime - サブスクリプションの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="3feeb-189">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="3feeb-190">clientState - サブスクリプション要求で指定された clientState プロパティ。</span><span class="sxs-lookup"><span data-stu-id="3feeb-190">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="3feeb-p111">changeType - 通知の原因となったイベントの種類。たとえば、メール受信時は *created*、メッセージの既読マークが付いたときに *updated* などです。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="3feeb-193">resource - `https://graph.microsoft.com` に関連したリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="3feeb-193">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="3feeb-p112">resourceData - 登録されているリソースに依存したオブジェクト。たとえば、Outlook リソースの場合は次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="3feeb-196">@odata.type - 表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。</span><span class="sxs-lookup"><span data-stu-id="3feeb-196">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="3feeb-197">@odata.id - オブジェクトの OData 識別子。</span><span class="sxs-lookup"><span data-stu-id="3feeb-197">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="3feeb-198">@odata.etag - オブジェクトのバージョンを表す HTTP エンティティ タグ。</span><span class="sxs-lookup"><span data-stu-id="3feeb-198">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="3feeb-199">id - オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="3feeb-199">id - The identifier of the object.</span></span>

> <span data-ttu-id="3feeb-p113">注:resourceData で指定される Id の値は、通知がキューに置かれたときに有効です。メッセージを別のフォルダーに移動するなどの一部のアクションでは、リソースの Id が変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

### <a name="notification-example"></a><span data-ttu-id="3feeb-202">通知の例</span><span class="sxs-lookup"><span data-stu-id="3feeb-202">Notification example</span></span>

<span data-ttu-id="3feeb-203">ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-203">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

``` json
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "id":"<long_id_string>"
    }
  }
  ]
}
```

<span data-ttu-id="3feeb-p114">値オブジェクトにリストが含まれていることに注意してください。キューに入っている通知が多い場合、Microsoft Graph は 1 つの要求でそれらを送信します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p114">Note the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="3feeb-206">通知の処理</span><span class="sxs-lookup"><span data-stu-id="3feeb-206">Processing the notification</span></span>

<span data-ttu-id="3feeb-p115">アプリケーションは通知の受信を開始すると、それらを処理する必要があります。アプリが通知を処理するために必要な最小限のタスクは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="3feeb-p116">`clientState` プロパティを検証します。通知の clientState プロパティは、サブスクリプション要求で送信されたプロパティと一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="3feeb-p117">注:一致しない場合、これを有効な通知と見なすことはできません。また、通知の送信元を調査し、適切なアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="3feeb-213">ビジネス ロジックに基づいて、アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-213">Update your application based on your business logic.</span></span>

3. <span data-ttu-id="3feeb-p118">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。Microsoft Graph が 2xx クラス コードを受信しない場合は、通知の再送信を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="3feeb-216">clientState プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3feeb-216">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="3feeb-217">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="3feeb-217">Repeat for other notifications in the request.</span></span>

## <a name="see-also"></a><span data-ttu-id="3feeb-218">関連項目</span><span class="sxs-lookup"><span data-stu-id="3feeb-218">See also</span></span>

* [<span data-ttu-id="3feeb-219">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="3feeb-219">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
* [<span data-ttu-id="3feeb-220">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="3feeb-220">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
* [<span data-ttu-id="3feeb-221">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="3feeb-221">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [<span data-ttu-id="3feeb-222">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="3feeb-222">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="3feeb-223">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="3feeb-223">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[連絡先]: ../api-reference/v1.0/resources/contact.md
[contact]: ../api-reference/v1.0/resources/contact.md
[会話]: ../api-reference/v1.0/resources/conversation.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[ドライブ]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
[イベント]: ../api-reference/v1.0/resources/event.md
[event]: ../api-reference/v1.0/resources/event.md
[メッセージ]: ../api-reference/v1.0/resources/message.md
[message]: ../api-reference/v1.0/resources/message.md
