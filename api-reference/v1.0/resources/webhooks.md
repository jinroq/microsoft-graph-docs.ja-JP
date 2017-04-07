# <a name="working-with-webhooks-in-microsoft-graph"></a>Microsoft Graph の Webhooks での作業

Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。

Microsoft Graph の REST API を使用すると、アプリは次のリソースに変更を登録できます。

* Messages
* イベント
* 連絡先
* グループ会話
* ドライブ ルート項目

Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。アプリはその後、そのビジネス ロジックに従ってアクションを実行します。たとえば、詳細データのフェッチ、キャッシュやビューの更新などです。

アプリは、期限が切れる前にサブスクリプションを更新する必要があります。また、いつでも登録を解除して、通知の受信を停止できます。

GitHub の次のコード サンプルを参照してください。

* [Node.js 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [ASP.NET 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

サブスクリプション プロセスを見てみましょう。

# <a name="creating-a-subscription"></a>サブスクリプションの作成

リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。

1. クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。
2. Microsoft Graph が要求を確認します。
  * 要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。
  * 要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。
3. クライアントは、Microsoft Graph に検証トークンを返送します。

クライアントは、対応するサブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。

## <a name="characteristics-of-subscriptions"></a>サブスクリプションの特性

メッセージ、イベント、連絡先、ドライブ ルート項目などのリソースについて、サブスクリプションを作成できます。

特定のフォルダーへのサブスクリプションを作成できます。`https://graph.microsoft.com/v1.0/me/mailfolders('inbox')/messages`

または最上位レベルのリソースへのサブスクリプションを作成できます。`https://graph.microsoft.com/v1.0/me/messages`

または、ドライブ ルート項目のサブスクリプションを作成できます。`https://graph.microsoft.com/v1.0/me/drive/root`

ほとんどの場合、サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。たとえば、通知メッセージを受信するには、アプリに `mail.read` アクセス許可が必要です。現在、OneDrive のドライブ ルート項目には `Files.ReadWrite` アクセス許可が必要であり、SharePoint サイトに関連付けられたドライブには `Files.ReadWrite.All` が必要であることに注意してください。

サブスクリプションには有効期限があります。現在の最長有効期限は、作成時から 3 日間から 90 分を引いた期間です (合計 4230 分)。アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。そうしない場合、新しいサブスクリプションを作成する必要があります。

## <a name="notification-url-validation"></a>通知 URL の検証

Microsoft Graph は、サブスクリプションを作成する前にサブスクリプション要求の通知 URL を検証します。検証プロセスは、次のようになります。

1. Microsoft Graph が通知 URL に POST 要求を送信します。

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。

  * 200 (OK) ステータス コード。
  * コンテンツ タイプはテキスト/書式なしである必要があります。 
  * 本文には Microsoft Graph が提供した検証トークンを含める必要があります。

クライアントは、応答を提供した後は検証トークンを破棄する必要があります。

## <a name="subscription-request-example"></a>サブスクリプション要求の例

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

changeType、notificationUrl、resource、および expirationDateTime の各プロパティは必須です。プロパティの定義と値については、「[サブスクリプション リソースの種類](subscription.md)」をご覧ください。clientState は必須ではありませんが、推奨される通知の処理プロセスに準拠するためには含める必要があります。

処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](subscription.md) オブジェクトを返します。

# <a name="renewing-a-subscription"></a>サブスクリプションの更新

クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。expirationDateTime プロパティは必須です。

## <a name="subscription-renewal-example"></a>サブスクリプションの更新の例

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](subscription.md) オブジェクトを返します。サブスクリプション オブジェクトには、新しい expirationDateTime の値が含まれています。 

# <a name="deleting-a-subscription"></a>サブスクリプションの削除

クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。

# <a name="notifications"></a>通知

クライアントはサブスクリプションを作成した後、通知の受信を開始します。Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。クライアントは、指定した変更の種類 (*created* など) に応じた通知のみを受信します。

## <a name="notification-properties"></a>通知のプロパティ

通知オブジェクトには、次のプロパティがあります。

* id - この通知が属するサブスクリプションの ID。
* expirationDateTime - サブスクリプションの有効期限が切れるとき。
* clientState - サブスクリプション要求で指定された clientState プロパティ。
* changeType - 通知の原因となったイベントの種類。たとえば、メール受信時は *created*、メッセージの既読マークが付いたときに *updated* などです。
* resource - `https://graph.microsoft.com` に関連したリソースの URI。 
* resourceData - 登録されているリソースに依存したオブジェクト。たとえば、Outlook リソースの場合は次のようなものがあります。
  * @odata.type - 表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。
  * @odata.id - オブジェクトの OData 識別子。
  * @odata.etag - オブジェクトのバージョンを表す HTTP エンティティ タグ。
  * Id - オブジェクトの識別子。


> 注:resourceData で指定される Id の値は、通知がキューに置かれたときに有効です。メッセージを別のフォルダーに移動するなどの一部のアクションでは、リソースの Id が変更される可能性があります。 

## <a name="notification-example"></a>通知の例

ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。

```
{
  "value":[
  {
    "id":"<subscription_guid>",
    "expirationDateTime":"\"2016-03-19T22:11:09.952Z\"",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "Id":"<long_id_string>"
    }
  }
  ]
}
```

値オブジェクトにリストが含まれていることに注意してください。キューに入っている通知が多い場合、Microsoft Graph は 1 つの要求でそれらを送信します。

## <a name="processing-the-notification"></a>通知の処理

アプリケーションは通知の受信を開始すると、それらを処理する必要があります。アプリが通知を処理するために必要な最小限のタスクは、次のようになります。

1. `clientState` プロパティを検証します。通知の clientState プロパティは、サブスクリプション要求で送信されたプロパティと一致する必要があります。
  > 注:一致しない場合、これを有効な通知と見なすことはできません。また、通知の送信元を調査し、適切なアクションを実行する必要があります。

2. ビジネス ロジックに基づいて、アプリケーションを更新します。
3. Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。Microsoft Graph が 2xx クラス コードを受信しない場合は、通知の再送信を何回でも再試行します。
  > clientState プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。

要求内の他の通知について、これらを繰り返します。

# <a name="additional-resources"></a>その他の技術情報

* [サブスクリプション リソースの種類](subscription.md)
* [サブスクリプションを取得する](../api/subscription_get.md)
* [サブスクリプションを作成する](../api/subscription_post_subscriptions.md)
* [Node.js 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [ASP.NET 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
