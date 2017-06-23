# <a name="create-subscription"></a>サブスクリプションを作成する

Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。
## <a name="prerequisites"></a>前提条件
この API を実行するためには、対象のリソースに応じた、次のいずれかの**スコープ**が必要です。*Mail.Read*、*Calendars.Read*、*Contacts.Read*、*Group.Read.All*、*Files.ReadWrite*、または *Files.ReadWrite.All*。***注:***/V1.0 エンドポイントでは、リソースのほとんどに対してアプリケーションのアクセス許可があります。グループ内の会話と OneDrive のドライブのルート項目は、アプリケーションのアクセス許可ではサポートされていません。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |


## <a name="response"></a>応答
成功した場合、このメソッドは `201, Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
ユーザーが新しいメールを受信したときに通知を送信する要求の例を次に示します。
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
要求本文で、[subscription](../resources/subscription.md) オブジェクトの JSON 表記を指定します。*clientState* フィールドはオプションです。

##### <a name="resources-examples"></a>リソースの例
以下は、サブスクリプションのリソース プロパティの有効な値です。

| リソースの種類 | 例 |
|:------ |:----- |
|メール|me/mailfolders('inbox')/messages<br />me/messages|
|連絡先|me/contacts|
|カレンダー|me/events|
|会話|groups('*{id}*')/conversations|
|ドライブ|me/drive/root|

##### <a name="response"></a>応答
以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
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
## <a name="subscription-validation"></a>サブスクリプションの検証
任意の URL へ通知を送信する誤ったサブスクリプションを回避するため、サブスクリプション通知エンドポイントは検証要求に応答できなければなりません。`/subscriptions` エンドポイントへの `POST` の処理中に、Microsoft Graph は `POST` 要求を次の形式で `notificationUrl` へ送り返します。 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
通知エンドポイントは、本文に値 `<token>` が入った、コンテンツ タイプが `text/plain` の 200 応答 (以下に示します) を 10 秒以内に送信しなければなりません。さもないと、作成要求は破棄されます。
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
##### <a name="notification-payload"></a>通知のペイロード
登録されたリソースが変更されると、webhook 機能が、次のペイロードで通知 URL に通知を送信します。通知エンドポイントは、30 秒以内に 200 または 204 の応答を応答本文なしで送信する必要があります。さもないと、指数関数的に増加する間隔で通知が再試行されます。いつも 30 秒以上かかるサービスの場合は、調整されて、より広い間隔で一連の通知を受け取ることがあります。

サービスは通知から 422 の応答を返すこともできます。この場合、サブスクリプションは自動的に削除され、通知のストリームが停止します。

登録されたリソースによっては、追加の resourceData フィールドが追加情報を提供する可能性があります。

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
ドライブ サブスクリプションから通知を受信した場合は、resourceData が null になるため、[差分](item_delta.md) API を呼び出して、発生した変更を判別しなければなりません。ドライブ通知の例を次に示します。
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
