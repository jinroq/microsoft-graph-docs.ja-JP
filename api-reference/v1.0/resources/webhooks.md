# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Microsoft Graph API を使用して変更通知を取得するには

Microsoft Graph の REST API は、Webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 受信通知を購読・処理する方法の詳細については、「[ユーザー データの変更に関する通知の設定](../../../concepts/webhooks.md)」を参照してください。

Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。

- メッセージ
- イベント
- 連絡先
- ユーザー
- グループ
- グループ会話
- SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ
- ユーザーの個人用 OneDrive フォルダー

## <a name="permissions"></a>アクセス許可

一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription_post_subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。

| アクセス許可の種類                        | v1.0 でサポートされているリソース                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| 委任 - 職場または学校アカウント     | [連絡先][]、[スレッド][]、[ドライブ][]、[イベント][]、[メッセージ][] |
| 委任 - 個人用の Microsoft アカウント | なし                                                             |
| アプリケーション                            | [連絡先][]、[スレッド][]、[イベント][]、[メッセージ][]            |

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](./subscription.md)
- [サブスクリプションを取得する](../api/subscription_get.md)
- [サブスクリプションを作成する](../api/subscription_post_subscriptions.md)
- [サブスクリプションを更新する](../api/subscription_update.md)
- [サブスクリプションを削除する](../api/subscription_delete.md)

[連絡先]: ./contact.md
[会話]: ./conversation.md
[ドライブ]: ./drive.md
[イベント]: ./event.md
[メッセージ]: ./message.md
