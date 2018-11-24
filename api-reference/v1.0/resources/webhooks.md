# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>変更通知を使用して Microsoft グラフ API を取得するには

Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](../../../concepts/webhooks.md)を参照してください。

Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。

- メッセージ
- イベント
- 連絡先
- ユーザー
- グループ
- グループ会話
- SharePoint サイトに関連付けられているドライブを含む、OneDrive で共有されているコンテンツ
- ユーザーの個人用の OneDrive フォルダー
- セキュリティの警告

## <a name="permissions"></a>アクセス許可

一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。

| アクセス許可の種類                        | v1.0 でサポートされているリソース                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| 委任 - 職場または学校アカウント     | [お問い合わせください][]、[会話][]、[ドライブ][]、[イベント][]、[メッセージ][]、[警告][] |
| 委任 - 個人用の Microsoft アカウント | なし                                                             |
| アプリケーション                            | [お問い合わせください][]、[会話][]、[イベント][]、[メッセージ][]、[警告][]           |

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](./subscription.md)
- [サブスクリプションを取得する](../api/subscription_get.md)
- [サブスクリプションを作成する](../api/subscription_post_subscriptions.md)
- [Update subscription](../api/subscription_update.md)
- [サブスクリプションの削除](../api/subscription_delete.md)

[連絡先]: ./contact.md
[会話]: ./conversation.md
[ドライブ]: ./drive.md
[イベント]: ./event.md
[メッセージ]: ./message.md
[アラート]: ./alert.md