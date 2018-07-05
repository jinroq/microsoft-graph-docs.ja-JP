# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="f614f-101">ユーザー データの変更に関する通知の設定</span><span class="sxs-lookup"><span data-stu-id="f614f-101">Set up notifications for changes in user data</span></span>

<span data-ttu-id="f614f-p101">Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="f614f-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="f614f-105">Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。</span><span class="sxs-lookup"><span data-stu-id="f614f-105">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span> <span data-ttu-id="f614f-106">アプリはその後、そのビジネス ロジックに従ってアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="f614f-106">The app then takes action according to its business logic.</span></span> <span data-ttu-id="f614f-107">たとえば、詳細データのフェッチ、そのキャッシュやビューの更新などです。</span><span class="sxs-lookup"><span data-stu-id="f614f-107">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="f614f-108">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="f614f-108">Supported resources</span></span>

<span data-ttu-id="f614f-109">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="f614f-109">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="f614f-110">メッセージ</span><span class="sxs-lookup"><span data-stu-id="f614f-110">Messages</span></span>
- <span data-ttu-id="f614f-111">イベント</span><span class="sxs-lookup"><span data-stu-id="f614f-111">Events</span></span>
- <span data-ttu-id="f614f-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="f614f-112">Contacts</span></span>
- <span data-ttu-id="f614f-113">ユーザー</span><span class="sxs-lookup"><span data-stu-id="f614f-113">Users</span></span>
- <span data-ttu-id="f614f-114">グループ</span><span class="sxs-lookup"><span data-stu-id="f614f-114">Groups</span></span>
- <span data-ttu-id="f614f-115">グループ会話</span><span class="sxs-lookup"><span data-stu-id="f614f-115">Group conversations</span></span>
- <span data-ttu-id="f614f-116">SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="f614f-116">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="f614f-117">ユーザーの個人用 OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="f614f-117">User's personal OneDrive folders</span></span>

<span data-ttu-id="f614f-118">たとえば、特定のメール フォルダーへサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="f614f-118">For instance, you can create a subscription to a specific folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="f614f-119">あるいは、最上位レベルのリソース: `me/messages`、`me/contacts`、`me/events`、`users`、または `groups`</span><span class="sxs-lookup"><span data-stu-id="f614f-119">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="f614f-120">あるいは、特定のリソース インスタンス: `users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="f614f-120">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="f614f-121">あるいは、Sharepoint/OneDrive for Business ドライブ: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="f614f-121">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="f614f-122">あるいは、ユーザーの個人用 OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="f614f-122">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="f614f-123">Azure AD リソースの制限</span><span class="sxs-lookup"><span data-stu-id="f614f-123">Azure AD Resource Limitations</span></span>

<span data-ttu-id="f614f-124">Azure AD ベースのリソース (ユーザー、グループ) には一定の制限が適用され、超過するとエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-124">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="f614f-125">最大サブスクリプションのクォータ:</span><span class="sxs-lookup"><span data-stu-id="f614f-125">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="f614f-126">アプリあたり: 合計 50,000 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f614f-126">Per App: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="f614f-127">テナントあたり: すべてのアプリで合計 35 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f614f-127">Per Tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="f614f-128">アプリとテナントの組み合わせ: 合計 7 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f614f-128">Per App and Tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="f614f-129">Azure AD B2C テナントはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f614f-129">Azure AD B2C tenants are not supported</span></span>

- <span data-ttu-id="f614f-130">ユーザー エンティティの通知は、個人用 Microsoft アカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f614f-130">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="f614f-131">サブスクリプション ライフタイム</span><span class="sxs-lookup"><span data-stu-id="f614f-131">Subscription lifetime</span></span>

<span data-ttu-id="f614f-132">サブスクリプションのライフタイムには制限があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-132">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="f614f-133">アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-133">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="f614f-134">そうしない場合、新しいサブスクリプションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-134">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="f614f-135">最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f614f-135">For a list of maximum expiration times, see [Maximum length of subscription per resource type](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="f614f-136">また、アプリはいつでも登録を解除して、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="f614f-136">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="f614f-137">サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f614f-137">Managing subscriptions</span></span>

<span data-ttu-id="f614f-138">クライアントは、サブスクリプションを作成したり、サブスクリプションを更新したり、サブスクリプションを削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="f614f-138">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="f614f-139">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="f614f-139">Creating a subscription</span></span>

<span data-ttu-id="f614f-p104">リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f614f-p104">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="f614f-142">クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-142">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="f614f-143">Microsoft Graph が要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="f614f-143">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="f614f-144">要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-144">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="f614f-145">要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-145">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="f614f-146">クライアントは、Microsoft Graph に検証トークンを返送します。</span><span class="sxs-lookup"><span data-stu-id="f614f-146">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="f614f-147">Microsoft Graph からクライアントに応答が送信されます。</span><span class="sxs-lookup"><span data-stu-id="f614f-147">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="f614f-148">クライアントは、サブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="f614f-149">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="f614f-149">Subscription request example</span></span>

```http
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

<span data-ttu-id="f614f-150">プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。</span><span class="sxs-lookup"><span data-stu-id="f614f-150">The `changeType`, `notificationUrl`, `resource` and `expirationDateTime` properties are required while the rest are optional.</span></span> <span data-ttu-id="f614f-151">プロパティの定義と値については、「[サブスクリプション リソースの種類](../api-reference/v1.0/resources/subscription.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f614f-151">See [subscription resource type](../api-reference/v1.0/resources/subscription.md) for property definitions and values.</span></span>

<span data-ttu-id="f614f-152">`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-152">The , , , and  properties are required. See subscription resource type for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="f614f-153">このプロパティを設定すると、受け取る通知が Microsoft Graph サービスから来たものであることを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="f614f-153">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="f614f-154">その理由で、このプロパティの値は機密として保たなければならず、使用はアプリケーションと Microsoft Graph サービスのためにのみ限るようにしてください。</span><span class="sxs-lookup"><span data-stu-id="f614f-154">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="f614f-155">処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](../api-reference/v1.0/resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f614f-155">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="f614f-156">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="f614f-156">Notification endpoint validation</span></span>

<span data-ttu-id="f614f-157">Microsoft Graph により、サブスクリプション作成の前にサブスクリプション要求の `notificationUrl` プロパティの中で提供される通知エンドポイントが検証されます。</span><span class="sxs-lookup"><span data-stu-id="f614f-157">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="f614f-158">検証プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f614f-158">The filtering process in a dashboard occurs as follows:</span></span>

1. <span data-ttu-id="f614f-159">Microsoft Graph が通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-159">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ```

1. <span data-ttu-id="f614f-160">クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-160">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="f614f-161">200 (OK) 状態コード。</span><span class="sxs-lookup"><span data-stu-id="f614f-161">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="f614f-162">コンテンツ タイプは `text/plain` でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f614f-162">The content type must be text/plain.</span></span>
    - <span data-ttu-id="f614f-163">本文には Microsoft Graph が提供した検証トークンを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-163">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="f614f-164">クライアントは、応答を提供した後は検証トークンを破棄する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-164">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="f614f-165">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="f614f-165">Renewing a subscription</span></span>

<span data-ttu-id="f614f-166">クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。</span><span class="sxs-lookup"><span data-stu-id="f614f-166">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span> <span data-ttu-id="f614f-167">`expirationDateTime` プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="f614f-167">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="f614f-168">サブスクリプションの更新の例</span><span class="sxs-lookup"><span data-stu-id="f614f-168">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="f614f-169">処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](../api-reference/v1.0/resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f614f-169">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](../api-reference/v1.0/resources/subscription.md) object in the body.</span></span> <span data-ttu-id="f614f-170">サブスクリプション オブジェクトには、新しい `expirationDateTime` 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f614f-170">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="f614f-171">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="f614f-171">Deleting a subscription</span></span>

<span data-ttu-id="f614f-172">クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="f614f-172">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="f614f-173">処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f614f-173">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="f614f-174">通知</span><span class="sxs-lookup"><span data-stu-id="f614f-174">Notifications</span></span>

<span data-ttu-id="f614f-175">クライアントはサブスクリプションを作成した後、通知の受信を開始します。</span><span class="sxs-lookup"><span data-stu-id="f614f-175">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="f614f-176">Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-176">Microsoft Graph sends a POST request to the notification URL:</span></span> <span data-ttu-id="f614f-177">通知が送信されるのは、`created` など、サブスクリプションで指定されているタイプの変更についてのみです。</span><span class="sxs-lookup"><span data-stu-id="f614f-177">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="f614f-178">**注:** 同じリソース タイプを監視し、同じ通知 URL を使用する複数のサブスクリプションを使用している場合、サブスクリプション ID が異なる複数の通知が含まれる POST が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f614f-178">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="f614f-179">その POST に含まれるすべての通知が、単一のサブスクリプションに属しているという保証はありません。</span><span class="sxs-lookup"><span data-stu-id="f614f-179">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="f614f-180">通知のプロパティ</span><span class="sxs-lookup"><span data-stu-id="f614f-180">Notification properties</span></span>

<span data-ttu-id="f614f-181">通知オブジェクトには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="f614f-181">The notification object has the following properties:</span></span>

| <span data-ttu-id="f614f-182">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f614f-182">Property</span></span> | <span data-ttu-id="f614f-183">型</span><span class="sxs-lookup"><span data-stu-id="f614f-183">Type</span></span> | <span data-ttu-id="f614f-184">説明</span><span class="sxs-lookup"><span data-stu-id="f614f-184">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f614f-185">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f614f-185">SubscriptionId</span></span> | <span data-ttu-id="f614f-186">string</span><span class="sxs-lookup"><span data-stu-id="f614f-186">string</span></span> | <span data-ttu-id="f614f-187">通知を生成したサブスクリプションの ID。</span><span class="sxs-lookup"><span data-stu-id="f614f-187">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="f614f-188">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f614f-188">SubscriptionExpirationDateTime</span></span> | [<span data-ttu-id="f614f-189">dateTime</span><span class="sxs-lookup"><span data-stu-id="f614f-189">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f614f-190">サブスクリプションの有効期限が切れるとき。</span><span class="sxs-lookup"><span data-stu-id="f614f-190">: The expiration time for the subscription.</span></span> |
| <span data-ttu-id="f614f-191">clientState</span><span class="sxs-lookup"><span data-stu-id="f614f-191">clientState</span></span> | <span data-ttu-id="f614f-192">string</span><span class="sxs-lookup"><span data-stu-id="f614f-192">string</span></span> | <span data-ttu-id="f614f-193">サブスクリプション要求で指定された `clientState` プロパティ (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="f614f-193">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="f614f-194">changeType</span><span class="sxs-lookup"><span data-stu-id="f614f-194">changeType</span></span> | <span data-ttu-id="f614f-195">string</span><span class="sxs-lookup"><span data-stu-id="f614f-195">string</span></span> | <span data-ttu-id="f614f-196">通知の原因となったイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="f614f-196">The event type that caused the notification.</span></span> <span data-ttu-id="f614f-197">たとえば、メール受信時は `created`、または読んだメッセージをマークした場合は `updated`。</span><span class="sxs-lookup"><span data-stu-id="f614f-197">changeType - The event type that caused the notification. For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="f614f-198">resource</span><span class="sxs-lookup"><span data-stu-id="f614f-198">resource</span></span> | <span data-ttu-id="f614f-199">string</span><span class="sxs-lookup"><span data-stu-id="f614f-199">string</span></span> | <span data-ttu-id="f614f-200">`https://graph.microsoft.com` に関連するリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="f614f-200">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="f614f-201">resourceData</span><span class="sxs-lookup"><span data-stu-id="f614f-201">ResourceData</span></span> | <span data-ttu-id="f614f-202">object</span><span class="sxs-lookup"><span data-stu-id="f614f-202">object</span></span> | <span data-ttu-id="f614f-203">このプロパティの内容は、サブスクリプションの対象となるリソースの種類に応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="f614f-203">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="f614f-204">たとえば、Outlook リソースの場合、`resourceData` には次のフィールドが含まれています:</span><span class="sxs-lookup"><span data-stu-id="f614f-204">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="f614f-205">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f614f-205">Property</span></span> | <span data-ttu-id="f614f-206">型</span><span class="sxs-lookup"><span data-stu-id="f614f-206">Type</span></span> | <span data-ttu-id="f614f-207">説明</span><span class="sxs-lookup"><span data-stu-id="f614f-207">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f614f-208">@odata.type</span><span class="sxs-lookup"><span data-stu-id="f614f-208">@odata.type</span></span> | <span data-ttu-id="f614f-209">string</span><span class="sxs-lookup"><span data-stu-id="f614f-209">string</span></span> | <span data-ttu-id="f614f-210">表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。</span><span class="sxs-lookup"><span data-stu-id="f614f-210">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="f614f-211">@odata.id</span><span class="sxs-lookup"><span data-stu-id="f614f-211">@odata.id</span></span> | <span data-ttu-id="f614f-212">string</span><span class="sxs-lookup"><span data-stu-id="f614f-212">string</span></span> | <span data-ttu-id="f614f-213">オブジェクトの OData 識別子。</span><span class="sxs-lookup"><span data-stu-id="f614f-213">@odata.id - The OData identifier of the object.</span></span> |
| <span data-ttu-id="f614f-214">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="f614f-214">@odata.etag</span></span> | <span data-ttu-id="f614f-215">string</span><span class="sxs-lookup"><span data-stu-id="f614f-215">string</span></span> | <span data-ttu-id="f614f-216">オブジェクトのバージョンを表す HTTP エンティティ タグ。</span><span class="sxs-lookup"><span data-stu-id="f614f-216">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span> |
| <span data-ttu-id="f614f-217">ID</span><span class="sxs-lookup"><span data-stu-id="f614f-217">id</span></span> | <span data-ttu-id="f614f-218">string</span><span class="sxs-lookup"><span data-stu-id="f614f-218">string</span></span> | <span data-ttu-id="f614f-219">オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="f614f-219">Id - The identifier of the object.</span></span> |

> <span data-ttu-id="f614f-220">**注:** `resourceData` で提供される `id` 値は、通知生成時に有効だったものです。</span><span class="sxs-lookup"><span data-stu-id="f614f-220">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="f614f-221">メッセージを別のフォルダーに移動するなど、アクションによっては、通知処理時に `id` が有効でなくなるという結果になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-221">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="f614f-222">通知の例</span><span class="sxs-lookup"><span data-stu-id="f614f-222">Notification example</span></span>

<span data-ttu-id="f614f-223">ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-223">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
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

<span data-ttu-id="f614f-224">`value` フィールドはオブジェクトの配列であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f614f-224">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="f614f-225">キューに多数の通知が入っている場合、Microsoft Graph から、単一の要求の中で複数の項目が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f614f-225">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="f614f-226">同じ通知要求の中に、異なる複数のサブスクリプションからの通知が含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="f614f-226">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="f614f-227">通知の処理</span><span class="sxs-lookup"><span data-stu-id="f614f-227">Processing the notification</span></span>

<span data-ttu-id="f614f-228">アプリの受け取る通知を、それぞれ処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-228">Each notification received by your app should be processed.</span></span> <span data-ttu-id="f614f-229">アプリが通知を処理するために必要な最小限のタスクは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="f614f-229">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="f614f-230">`clientState` プロパティを検証します。</span><span class="sxs-lookup"><span data-stu-id="f614f-230">Validate the `clientState` property.</span></span> <span data-ttu-id="f614f-231">これは、サブスクリプション作成要求で当初送られた値に一致していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="f614f-231">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="f614f-232">**注:** そうでない場合、これを有効な通知と見なすことはできません。</span><span class="sxs-lookup"><span data-stu-id="f614f-232">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="f614f-233">通知が Microsoft Graph に由来するものでなく、悪意のある者が偽って送った可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-233">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="f614f-234">また、通知の送信元を調査し、適切なアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-234">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="f614f-235">ビジネス ロジックに基づいて、アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="f614f-235">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="f614f-236">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。</span><span class="sxs-lookup"><span data-stu-id="f614f-236">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="f614f-237">Microsoft Graph が 2xx クラス コードを受信しない場合は、通知を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="f614f-237">Send a  status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>

    > <span data-ttu-id="f614f-238">**注:** `clientState`プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f614f-238">You should send a  status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="f614f-239">これは、偽通知が信頼されていないかもしれないという事実を悪意のある者が検出し、それを利用して `clientState` プロパティの値を類推するのを防ぐことになるため、優れた方法と言えます。</span><span class="sxs-lookup"><span data-stu-id="f614f-239">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="f614f-240">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="f614f-240">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="f614f-241">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="f614f-241">Code samples</span></span>

<span data-ttu-id="f614f-242">GitHub では、次のコード サンプルを利用できます。</span><span class="sxs-lookup"><span data-stu-id="f614f-242">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="f614f-243">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="f614f-243">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="f614f-244">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="f614f-244">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="f614f-245">WebJobs SDK を使用した Microsoft Graph ユーザー Webhook のサンプル</span><span class="sxs-lookup"><span data-stu-id="f614f-245">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="f614f-246">関連項目</span><span class="sxs-lookup"><span data-stu-id="f614f-246">See also</span></span>

- [<span data-ttu-id="f614f-247">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="f614f-247">Subscription resource type</span></span>](../api-reference/v1.0/resources/subscription.md)
- [<span data-ttu-id="f614f-248">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="f614f-248">Get subscription</span></span>](../api-reference/v1.0/api/subscription_get.md)
- [<span data-ttu-id="f614f-249">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="f614f-249">Create subscription</span></span>](../api-reference/v1.0/api/subscription_post_subscriptions.md)

[contact]: ../api-reference/v1.0/resources/contact.md
[conversation]: ../api-reference/v1.0/resources/conversation.md
[drive]: ../api-reference/v1.0/resources/drive.md
[event]: ../api-reference/v1.0/resources/event.md
[message]: ../api-reference/v1.0/resources/message.md
