# <a name="subscription-resource-type"></a>Subscription リソースタイプ
サブスクリプションは、Microsoft Graph 上のデータに関する通知の受信をクライアントのアプリケーションに許可します。 サブスクリプションは現在、以下のデータセットで有効です:

1. Outlook からのメール、イベント、および連絡先
1. Office グループからの会話。
1. OneDrive からドライブ ルート項目 


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|changeType|string|登録しているリソース内の、通知を上げる変更の種類を示します。 サポートされている値は `created`、`updated`、`deleted` です。 コンマ区切りのリストを使用して複数値を結合できます。|
|notificationUrl|string|通知を受け取るエンドポイントの URL です。この URL は HTTPS プロトコルを利用する必要があります。|
|リソース|string|変更の監視対象となるリソースを指定します。ベース URL ("https://graph.microsoft.com/v1.0/") は含めないでください。|
|expirationDateTime|[dateTime](http://tools.ietf.org/html/rfc3339)|webhook サブスクリプションの有効期限が切れる日時を指定します。 時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。  サポートされているサブスクリプションの最長時間については、次の表をご覧ください。 |
|clientState|string|各通知内のサービスによって送信される `clientState` プロパティの値を指定します。 最大の長さは 128 文字です。 クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。|
|id|string|サブスクリプションの一意の識別子です。読み取り専用です。|

## <a name="maximum-length-of-subscription-per-resource-type"></a>リソースの種類別のサブスクリプションの最大の長さ
| リソース | 最大有効期限 |
|:---------------------|:--------------------|
|メール| 4230 分。|
|予定表| 4230 分。|
|連絡先| 4230 分。|
|グループ会話| 4230 分。|
|ドライブ ルート項目| 43200 分。 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。 今後のリリースでは、これより高い値は設定できません。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create subscription](../api/subscription_post_subscriptions.md) | [subscription](subscription.md) |Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。|
|[Update subscription](../api/subscription_update.md) | [subscription](subscription.md) |有効期限を更新することにより、サブスクリプションを更新します。|
|[Get subscription](../api/subscription_get.md) | [subscription](subscription.md) |サブスクリプション オブジェクトのプロパティと関係を読み取ります。|
|[サブスクリプションの削除](../api/subscription_delete.md) | なし |サブスクリプション オブジェクトを削除します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
