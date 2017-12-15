# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="d33fd-101">Microsoft Graph の Webhooks での作業</span><span class="sxs-lookup"><span data-stu-id="d33fd-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="d33fd-p101">Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="d33fd-105">Microsoft Graph の REST API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="d33fd-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="d33fd-106">Messages</span><span class="sxs-lookup"><span data-stu-id="d33fd-106">Messages</span></span>
* <span data-ttu-id="d33fd-107">イベント</span><span class="sxs-lookup"><span data-stu-id="d33fd-107">Events</span></span>
* <span data-ttu-id="d33fd-108">連絡先</span><span class="sxs-lookup"><span data-stu-id="d33fd-108">Contacts</span></span>
* <span data-ttu-id="d33fd-109">グループ会話</span><span class="sxs-lookup"><span data-stu-id="d33fd-109">Group conversations</span></span>
* <span data-ttu-id="d33fd-110">SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="d33fd-110">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="d33fd-111">ユーザーの個人用 OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="d33fd-111">User's personal OneDrive folders</span></span>

<span data-ttu-id="d33fd-112">たとえば、特定のフォルダーへのサブスクリプションを作成できます。`me/mailfolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="d33fd-112">For instance, you can create a subscription to a specific folder: `me/mailfolders('inbox')/messages`</span></span>

<span data-ttu-id="d33fd-113">最上位レベルのリソースへの場合は次のようになります。`me/messages`、`me/contacts`、`me/events`</span><span class="sxs-lookup"><span data-stu-id="d33fd-113">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`</span></span>

<span data-ttu-id="d33fd-114">Sharepoint/OneDrive for Business ドライブの場合は次のようになります。`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="d33fd-114">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="d33fd-115">ユーザーの個人用 OneDrive の場合は次のようになります。`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="d33fd-115">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="d33fd-p102">Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。アプリはその後、そのビジネス ロジックに従ってアクションを実行します。たとえば、詳細データのフェッチ、キャッシュやビューの更新などです。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="d33fd-119">アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-119">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="d33fd-120">そうしない場合、新しいサブスクリプションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-120">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="d33fd-121">最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](subscription.md#maximum-length-of-subscription-per-resource-type)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d33fd-121">For a list of maximum expiration times, see [Maximum length of subscription per resource type](subscription.md#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="d33fd-122">また、アプリはいつでも登録を解除して、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="d33fd-122">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="d33fd-p104">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="d33fd-127">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d33fd-127">Permission type</span></span> | <span data-ttu-id="d33fd-128">v1.0 でサポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="d33fd-128">Supported resource types in v1.0</span></span> |
|:----------------|:---------------------------------|
| <span data-ttu-id="d33fd-129">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="d33fd-129">Delegated - work or school account</span></span> | <span data-ttu-id="d33fd-130">[連絡先](contact.md)、[スレッド](conversation.md)、[ドライブ](drive.md)、[イベント](event.md)、[メッセージ](message.md)</span><span class="sxs-lookup"><span data-stu-id="d33fd-130">[contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message](message.md)</span></span> |
| <span data-ttu-id="d33fd-131">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="d33fd-131">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="d33fd-132">なし</span><span class="sxs-lookup"><span data-stu-id="d33fd-132">None</span></span> |
| <span data-ttu-id="d33fd-133">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d33fd-133">Application</span></span> | <span data-ttu-id="d33fd-134">[連絡先](contact.md)、[スレッド](conversation.md)、[イベント](event.md)、[メッセージ](message.md)</span><span class="sxs-lookup"><span data-stu-id="d33fd-134">[contact](contact.md), [conversation](conversation.md), [event](event.md), [message](message.md)</span></span> |

## <a name="code-samples"></a><span data-ttu-id="d33fd-135">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="d33fd-135">Code samples</span></span>

<span data-ttu-id="d33fd-136">GitHub では、次のコード サンプルを利用できます。</span><span class="sxs-lookup"><span data-stu-id="d33fd-136">The following code samples are available on GitHub.</span></span>

* [<span data-ttu-id="d33fd-137">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="d33fd-137">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="d33fd-138">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="d33fd-138">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

# <a name="creating-a-subscription"></a><span data-ttu-id="d33fd-139">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="d33fd-139">Creating a subscription</span></span>

<span data-ttu-id="d33fd-p105">リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="d33fd-142">クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-142">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="d33fd-143">Microsoft Graph が要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-143">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="d33fd-144">要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-144">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="d33fd-145">要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-145">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="d33fd-146">クライアントは、Microsoft Graph に検証トークンを返送します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-146">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="d33fd-147">クライアントは、対応するサブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-147">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

## <a name="notification-url-validation"></a><span data-ttu-id="d33fd-148">通知 URL の検証</span><span class="sxs-lookup"><span data-stu-id="d33fd-148">Notification URL validation</span></span>

<span data-ttu-id="d33fd-p106">Microsoft Graph は、サブスクリプションを作成する前にサブスクリプション要求の通知 URL を検証します。検証プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="d33fd-151">Microsoft Graph が通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-151">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. <span data-ttu-id="d33fd-152">クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-152">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="d33fd-153">200 (OK) 状態コード。</span><span class="sxs-lookup"><span data-stu-id="d33fd-153">A 200 (OK) status code.</span></span>
  * <span data-ttu-id="d33fd-154">コンテンツ タイプはテキスト/書式なしである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-154">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="d33fd-155">本文には Microsoft Graph が提供した検証トークンを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-155">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="d33fd-156">クライアントは、応答を提供した後は検証トークンを破棄する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-156">The client should discard the validation token after providing it in the response.</span></span>

## <a name="subscription-request-example"></a><span data-ttu-id="d33fd-157">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="d33fd-157">Subscription request example</span></span>

```
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

<span data-ttu-id="d33fd-p107">プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。プロパティの定義と値については、「[サブスクリプション リソースの種類](subscription.md)」をご覧ください。`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="d33fd-161">処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-161">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](subscription.md) object in the body.</span></span>

# <a name="renewing-a-subscription"></a><span data-ttu-id="d33fd-162">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="d33fd-162">Renewing a subscription</span></span>

<span data-ttu-id="d33fd-p108">クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。expirationDateTime プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

## <a name="subscription-renewal-example"></a><span data-ttu-id="d33fd-165">サブスクリプションの更新の例</span><span class="sxs-lookup"><span data-stu-id="d33fd-165">Subscription renewal example</span></span>

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="d33fd-p109">処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](subscription.md) オブジェクトを返します。サブスクリプション オブジェクトには、新しい expirationDateTime の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

# <a name="deleting-a-subscription"></a><span data-ttu-id="d33fd-168">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="d33fd-168">Deleting a subscription</span></span>

<span data-ttu-id="d33fd-169">クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="d33fd-169">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="d33fd-170">処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-170">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

# <a name="notifications"></a><span data-ttu-id="d33fd-171">通知</span><span class="sxs-lookup"><span data-stu-id="d33fd-171">Notifications</span></span>

<span data-ttu-id="d33fd-p110">クライアントはサブスクリプションを作成した後、通知の受信を開始します。Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。クライアントは、指定した変更の種類 (*created* など) に応じた通知のみを受信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

## <a name="notification-properties"></a><span data-ttu-id="d33fd-175">通知のプロパティ</span><span class="sxs-lookup"><span data-stu-id="d33fd-175">Notification properties</span></span>

<span data-ttu-id="d33fd-176">通知オブジェクトには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-176">The notification object has the following properties:</span></span>

* <span data-ttu-id="d33fd-177">subscriptionId - この通知が属するサブスクリプションの ID。</span><span class="sxs-lookup"><span data-stu-id="d33fd-177">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="d33fd-178">subscriptionExpirationDateTime - サブスクリプションの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="d33fd-178">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="d33fd-179">clientState - サブスクリプション要求で指定された clientState プロパティ。</span><span class="sxs-lookup"><span data-stu-id="d33fd-179">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="d33fd-p111">changeType - 通知の原因となったイベントの種類。たとえば、メール受信時は *created*、メッセージの既読マークが付いたときに *updated* などです。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="d33fd-182">resource - `https://graph.microsoft.com` に関連したリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="d33fd-182">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="d33fd-p112">resourceData - 登録されているリソースに依存したオブジェクト。たとえば、Outlook リソースの場合は次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="d33fd-185">@odata.type - 表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。</span><span class="sxs-lookup"><span data-stu-id="d33fd-185">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="d33fd-186">@odata.id - オブジェクトの OData 識別子。</span><span class="sxs-lookup"><span data-stu-id="d33fd-186">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="d33fd-187">@odata.etag - オブジェクトのバージョンを表す HTTP エンティティ タグ。</span><span class="sxs-lookup"><span data-stu-id="d33fd-187">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="d33fd-188">id - オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="d33fd-188">id - The identifier of the object.</span></span>


> <span data-ttu-id="d33fd-p113">注:resourceData で指定される Id の値は、通知がキューに置かれたときに有効です。メッセージを別のフォルダーに移動するなどの一部のアクションでは、リソースの Id が変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

## <a name="notification-example"></a><span data-ttu-id="d33fd-191">通知の例</span><span class="sxs-lookup"><span data-stu-id="d33fd-191">Notification example</span></span>

<span data-ttu-id="d33fd-192">ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-192">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```
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

<span data-ttu-id="d33fd-p114">値オブジェクトにリストが含まれていることに注意してください。キューに入っている通知が多い場合、Microsoft Graph は 1 つの要求でそれらを送信します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p114">Note the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

## <a name="processing-the-notification"></a><span data-ttu-id="d33fd-195">通知の処理</span><span class="sxs-lookup"><span data-stu-id="d33fd-195">Processing the notification</span></span>

<span data-ttu-id="d33fd-p115">アプリケーションは通知の受信を開始すると、それらを処理する必要があります。アプリが通知を処理するために必要な最小限のタスクは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="d33fd-p116">`clientState` プロパティを検証します。通知の clientState プロパティは、サブスクリプション要求で送信されたプロパティと一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="d33fd-p117">注:一致しない場合、これを有効な通知と見なすことはできません。また、通知の送信元を調査し、適切なアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="d33fd-202">ビジネス ロジックに基づいて、アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-202">Update your application based on your business logic.</span></span>
3. <span data-ttu-id="d33fd-p118">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。Microsoft Graph が 2xx クラス コードを受信しない場合は、通知の再送信を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="d33fd-205">clientState プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d33fd-205">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="d33fd-206">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="d33fd-206">Repeat for other notifications in the request.</span></span>

# <a name="additional-resources"></a><span data-ttu-id="d33fd-207">その他の技術情報</span><span class="sxs-lookup"><span data-stu-id="d33fd-207">Additional resources</span></span>

* [<span data-ttu-id="d33fd-208">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d33fd-208">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="d33fd-209">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="d33fd-209">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="d33fd-210">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="d33fd-210">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="d33fd-211">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="d33fd-211">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="d33fd-212">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="d33fd-212">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
