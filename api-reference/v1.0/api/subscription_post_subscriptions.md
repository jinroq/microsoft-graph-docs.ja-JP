# <a name="create-subscription"></a><span data-ttu-id="187c0-101">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="187c0-101">Create subscription</span></span>

<span data-ttu-id="187c0-102">Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="187c0-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="187c0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="187c0-103">Permissions</span></span>

<span data-ttu-id="187c0-p101">サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。たとえば、通知メッセージを受信するには、アプリに `Mail.Read` アクセス許可が必要です。次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="187c0-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="187c0-108">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="187c0-108">Resource type / Item</span></span>        | <span data-ttu-id="187c0-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="187c0-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="187c0-110">連絡先</span><span class="sxs-lookup"><span data-stu-id="187c0-110">Contacts</span></span>                    | <span data-ttu-id="187c0-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="187c0-111">Contacts.Read</span></span>       |
| <span data-ttu-id="187c0-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="187c0-112">Conversations</span></span>               | <span data-ttu-id="187c0-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="187c0-113">Group.Read.All</span></span>      |
| <span data-ttu-id="187c0-114">イベント</span><span class="sxs-lookup"><span data-stu-id="187c0-114">Events</span></span>                      | <span data-ttu-id="187c0-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="187c0-115">Calendars.Read</span></span>      |
| <span data-ttu-id="187c0-116">メッセージ</span><span class="sxs-lookup"><span data-stu-id="187c0-116">Messages</span></span>                    | <span data-ttu-id="187c0-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="187c0-117">Mail.Read</span></span>           |
| <span data-ttu-id="187c0-118">Groups</span><span class="sxs-lookup"><span data-stu-id="187c0-118">Groups</span></span>                      | <span data-ttu-id="187c0-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="187c0-119">Group.Read.All</span></span>      |
| <span data-ttu-id="187c0-120">Users</span><span class="sxs-lookup"><span data-stu-id="187c0-120">Users</span></span>                       | <span data-ttu-id="187c0-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="187c0-121">User.Read.All</span></span>       |
| <span data-ttu-id="187c0-122">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="187c0-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="187c0-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="187c0-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="187c0-124">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="187c0-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="187c0-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187c0-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="187c0-126">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="187c0-126">Security alert</span></span>| <span data-ttu-id="187c0-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187c0-127">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="187c0-128">**注:**/V1.0 エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="187c0-128">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="187c0-129">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="187c0-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="187c0-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="187c0-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="187c0-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="187c0-131">Request headers</span></span>

| <span data-ttu-id="187c0-132">名前</span><span class="sxs-lookup"><span data-stu-id="187c0-132">Name</span></span>       | <span data-ttu-id="187c0-133">型</span><span class="sxs-lookup"><span data-stu-id="187c0-133">Type</span></span> | <span data-ttu-id="187c0-134">説明</span><span class="sxs-lookup"><span data-stu-id="187c0-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="187c0-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="187c0-135">Authorization</span></span>  | <span data-ttu-id="187c0-136">string</span><span class="sxs-lookup"><span data-stu-id="187c0-136">string</span></span>  | <span data-ttu-id="187c0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="187c0-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="187c0-139">応答</span><span class="sxs-lookup"><span data-stu-id="187c0-139">Response</span></span>

<span data-ttu-id="187c0-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="187c0-140">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="187c0-141">例</span><span class="sxs-lookup"><span data-stu-id="187c0-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="187c0-142">要求</span><span class="sxs-lookup"><span data-stu-id="187c0-142">Request</span></span>

<span data-ttu-id="187c0-143">ユーザーが新しいメールを受信したときに通知を送信する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="187c0-143">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="187c0-144">要求の本文には、[サブスクリプション](../resources/subscription.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="187c0-144">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="187c0-145">`clientState`フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="187c0-145">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="187c0-146">リソースの例</span><span class="sxs-lookup"><span data-stu-id="187c0-146">Resources examples</span></span>

<span data-ttu-id="187c0-147">以下は、サブスクリプションのリソース プロパティの有効な値です。</span><span class="sxs-lookup"><span data-stu-id="187c0-147">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="187c0-148">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="187c0-148">Resource type</span></span> | <span data-ttu-id="187c0-149">例</span><span class="sxs-lookup"><span data-stu-id="187c0-149">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="187c0-150">メール</span><span class="sxs-lookup"><span data-stu-id="187c0-150">Mail</span></span>|<span data-ttu-id="187c0-151">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="187c0-151">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="187c0-152">me/messages</span><span class="sxs-lookup"><span data-stu-id="187c0-152">me/messages</span></span>|
|<span data-ttu-id="187c0-153">連絡先</span><span class="sxs-lookup"><span data-stu-id="187c0-153">Contacts</span></span>|<span data-ttu-id="187c0-154">me/contacts</span><span class="sxs-lookup"><span data-stu-id="187c0-154">me/contacts</span></span>|
|<span data-ttu-id="187c0-155">カレンダー</span><span class="sxs-lookup"><span data-stu-id="187c0-155">Calendars</span></span>|<span data-ttu-id="187c0-156">me/events</span><span class="sxs-lookup"><span data-stu-id="187c0-156">me/events</span></span>|
|<span data-ttu-id="187c0-157">Users</span><span class="sxs-lookup"><span data-stu-id="187c0-157">Users</span></span>|<span data-ttu-id="187c0-158">users</span><span class="sxs-lookup"><span data-stu-id="187c0-158">users</span></span>|
|<span data-ttu-id="187c0-159">Groups</span><span class="sxs-lookup"><span data-stu-id="187c0-159">Groups</span></span>|<span data-ttu-id="187c0-160">グループ</span><span class="sxs-lookup"><span data-stu-id="187c0-160">groups</span></span>|
|<span data-ttu-id="187c0-161">会話</span><span class="sxs-lookup"><span data-stu-id="187c0-161">Conversations</span></span>|<span data-ttu-id="187c0-162">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="187c0-162">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="187c0-163">ドライブ</span><span class="sxs-lookup"><span data-stu-id="187c0-163">Drives</span></span>|<span data-ttu-id="187c0-164">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="187c0-164">me/drive/root</span></span>|
|<span data-ttu-id="187c0-165">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="187c0-165">Security alert</span></span>|<span data-ttu-id="187c0-166">セキュリティと警告? $filter eq のステータスを 'New' =</span><span class="sxs-lookup"><span data-stu-id="187c0-166">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="187c0-167">応答</span><span class="sxs-lookup"><span data-stu-id="187c0-167">Response</span></span>

<span data-ttu-id="187c0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="187c0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="187c0-171">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="187c0-171">Notification endpoint validation</span></span>

<span data-ttu-id="187c0-172">サブスクリプション通知エンドポイント (で指定されている、`notificationUrl`プロパティ) の[ユーザー データの変更の通知の設定](../../../concepts/webhooks.md#notification-endpoint-validation)で説明したように、検証要求に応答できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="187c0-172">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="187c0-173">検証が失敗した場合、サブスクリプションを作成する要求は 400 不正な要求のエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="187c0-173">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
