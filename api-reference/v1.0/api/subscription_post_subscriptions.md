# <a name="create-subscription"></a><span data-ttu-id="60171-101">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="60171-101">Create subscription</span></span>

<span data-ttu-id="60171-102">Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="60171-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60171-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="60171-103">Prerequisites</span></span>
<span data-ttu-id="60171-p101">サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。たとえば、通知メッセージを受信するには、アプリに `Mail.Read` アクセス許可が必要です。次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="60171-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="60171-107">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="60171-107">Resource type / Item</span></span>        | <span data-ttu-id="60171-108">範囲</span><span class="sxs-lookup"><span data-stu-id="60171-108">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="60171-109">連絡先</span><span class="sxs-lookup"><span data-stu-id="60171-109">Contacts</span></span>                    | <span data-ttu-id="60171-110">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="60171-110">Contacts.Read</span></span>       |
| <span data-ttu-id="60171-111">スレッド</span><span class="sxs-lookup"><span data-stu-id="60171-111">Conversations</span></span>               | <span data-ttu-id="60171-112">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="60171-112">Group.Read.All</span></span>      |
| <span data-ttu-id="60171-113">イベント</span><span class="sxs-lookup"><span data-stu-id="60171-113">Events</span></span>                      | <span data-ttu-id="60171-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="60171-114">Calendars.Read</span></span>      |
| <span data-ttu-id="60171-115">メッセージ</span><span class="sxs-lookup"><span data-stu-id="60171-115">Messages</span></span>                    | <span data-ttu-id="60171-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="60171-116">Mail.Read</span></span>           |
| <span data-ttu-id="60171-117">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="60171-117">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="60171-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60171-118">Files.ReadWrite</span></span>     |
| <span data-ttu-id="60171-119">ドライブ (Sharepoint の共有コンテンツとドライブ)</span><span class="sxs-lookup"><span data-stu-id="60171-119">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="60171-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60171-120">Files.ReadWrite.All</span></span> |

 <span data-ttu-id="60171-p102">***メモ:***/V1.0 エンドポイントでは、リソースのほとんどに対してアプリケーションのアクセス許可があります。グループ内の会話と OneDrive のドライブのルート項目は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60171-p102">One of the following scopes, depending on the target resource, are required to execute this API: Mail.Read, Calendars.Read, Contacts.Read, Group.Read.All, Files.ReadWrite or Files.ReadWrite.All. ***Note:*** The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="60171-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60171-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a><span data-ttu-id="60171-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60171-124">Request headers</span></span>
| <span data-ttu-id="60171-125">名前</span><span class="sxs-lookup"><span data-stu-id="60171-125">Name</span></span>       | <span data-ttu-id="60171-126">型</span><span class="sxs-lookup"><span data-stu-id="60171-126">Type</span></span> | <span data-ttu-id="60171-127">説明</span><span class="sxs-lookup"><span data-stu-id="60171-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="60171-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="60171-128">Authorization</span></span>  | <span data-ttu-id="60171-129">string</span><span class="sxs-lookup"><span data-stu-id="60171-129">string</span></span>  | <span data-ttu-id="60171-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60171-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="60171-132">応答</span><span class="sxs-lookup"><span data-stu-id="60171-132">Response</span></span>

<span data-ttu-id="60171-133">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60171-133">If successful, this method returns `201, Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60171-134">例</span><span class="sxs-lookup"><span data-stu-id="60171-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60171-135">要求</span><span class="sxs-lookup"><span data-stu-id="60171-135">Request</span></span>
<span data-ttu-id="60171-136">ユーザーが新しいメールを受信したときに通知を送信する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60171-136">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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
   "clientState": "subscription-identifier"
}
```
<span data-ttu-id="60171-p104">要求本文で、[subscription](../resources/subscription.md) オブジェクトの JSON 表記を指定します。*clientState* フィールドはオプションです。</span><span class="sxs-lookup"><span data-stu-id="60171-p104">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object. The *clientState* field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="60171-139">リソースの例</span><span class="sxs-lookup"><span data-stu-id="60171-139">Resources examples</span></span>
<span data-ttu-id="60171-140">以下は、サブスクリプションのリソース プロパティの有効な値です。</span><span class="sxs-lookup"><span data-stu-id="60171-140">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="60171-141">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60171-141">Resource type</span></span> | <span data-ttu-id="60171-142">例</span><span class="sxs-lookup"><span data-stu-id="60171-142">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="60171-143">メール</span><span class="sxs-lookup"><span data-stu-id="60171-143">Mail</span></span>|<span data-ttu-id="60171-144">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="60171-144">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="60171-145">me/messages</span><span class="sxs-lookup"><span data-stu-id="60171-145">me/messages</span></span>|
|<span data-ttu-id="60171-146">連絡先</span><span class="sxs-lookup"><span data-stu-id="60171-146">Contacts</span></span>|<span data-ttu-id="60171-147">me/contacts</span><span class="sxs-lookup"><span data-stu-id="60171-147">me/contacts</span></span>|
|<span data-ttu-id="60171-148">カレンダー</span><span class="sxs-lookup"><span data-stu-id="60171-148">Calendars</span></span>|<span data-ttu-id="60171-149">me/events</span><span class="sxs-lookup"><span data-stu-id="60171-149">me/events</span></span>|
|<span data-ttu-id="60171-150">会話</span><span class="sxs-lookup"><span data-stu-id="60171-150">Conversations</span></span>|<span data-ttu-id="60171-151">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="60171-151">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="60171-152">ドライブ</span><span class="sxs-lookup"><span data-stu-id="60171-152">Drives</span></span>|<span data-ttu-id="60171-153">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="60171-153">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="60171-154">応答</span><span class="sxs-lookup"><span data-stu-id="60171-154">Response</span></span>
<span data-ttu-id="60171-p105">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="60171-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a><span data-ttu-id="60171-158">サブスクリプションの検証</span><span class="sxs-lookup"><span data-stu-id="60171-158">Subscription validation</span></span>
<span data-ttu-id="60171-p106">任意の URL へ通知を送信する誤ったサブスクリプションを回避するため、サブスクリプション通知エンドポイントは検証要求に応答できなければなりません。`/subscriptions` エンドポイントへの `POST` の処理中に、Microsoft Graph は `POST` 要求を次の形式で `notificationUrl` へ送り返します。</span><span class="sxs-lookup"><span data-stu-id="60171-p106">In order to to avoid mistaken subscriptions directing notifications to arbitrary URLs, the subscription notification endpoint must be capable of responding to a validation request. During processing of the `POST` to the `/subscriptions` endpoint, the Microsoft Graph will send a `POST` request back to your `notificationUrl` in the following form:</span></span> 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
<span data-ttu-id="60171-161">通知エンドポイントは、本文に値 `<token>` が入った、コンテンツ タイプが `text/plain` の 200 応答 (以下に示します) を 10 秒以内に送信しなければなりません。さもないと、作成要求は破棄されます。</span><span class="sxs-lookup"><span data-stu-id="60171-161">The notification endpoint must send a 200 response with the value of `<token>` as its body and a content type of `text/plain`, as shown below, within 10 seconds otherwise the creation request will be discarded.</span></span>
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a><span data-ttu-id="60171-162">通知のペイロード</span><span class="sxs-lookup"><span data-stu-id="60171-162">Notification payload</span></span>
<span data-ttu-id="60171-p107">登録されたリソースが変更されると、webhook 機能が、次のペイロードで通知 URL に通知を送信します。通知エンドポイントは、30 秒以内に 200 または 204 の応答を応答本文なしで送信する必要があります。さもないと、指数関数的に増加する間隔で通知が再試行されます。いつも 30 秒以上かかるサービスの場合は、調整されて、より広い間隔で一連の通知を受け取ることがあります。</span><span class="sxs-lookup"><span data-stu-id="60171-p107">When the subscribed resource changes, the webhooks facility sends a notification to your notification URL with the following payload.  The notification endpoint must send a response of 200 or 204 with no response body within 30 seconds otherwise the notification attempt will be retried at exponentially increasing intervals.  Services that consistently take 30 seconds or more may be throttled and receive a sparser notification set.</span></span>

<span data-ttu-id="60171-166">サービスは通知から 422 の応答を返すこともできます。この場合、サブスクリプションは自動的に削除され、通知のストリームが停止します。</span><span class="sxs-lookup"><span data-stu-id="60171-166">Services may also return a 422 response from a notification, in which case the subscription will be automatically deleted and the stream of notifications will come to a halt.</span></span>

<span data-ttu-id="60171-167">登録されたリソースによっては、追加の resourceData フィールドが追加情報を提供する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="60171-167">Depending on the subscribed resource, an additional resourceData field may provide additional information.</span></span>

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
<span data-ttu-id="60171-p108">ドライブ サブスクリプションから通知を受信した場合は、resourceData が null になるため、[差分](item_delta.md) API を呼び出して、発生した変更を判別しなければなりません。ドライブ通知の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60171-p108">When receiving notifications from Drive subscriptions the resourceData will be null and the [delta](item_delta.md) API should be called to determine the changes that have occured. Here is an example of a Drive notification:</span></span>
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
