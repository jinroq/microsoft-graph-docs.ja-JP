# <a name="subscription-resource-type"></a>サブスクリプション リソースの種類

サブスクリプションは、Microsoft Graph 上のデータに対する変更についての通知の受信をクライアント アプリケーションに許可します。 現時点では、サブスクリプションは次のリソースで有効です。

- Outlook からのメール、イベント、および連絡先
- Office グループからの会話。
- OneDrive からドライブ ルート項目
- Azure Active Directory からのユーザーおよびグループ

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ | タイプ | 説明 |
|:---------|:-----|:------------|
| changeType | 文字列 | 必須。 登録しているリソース内の、通知を上げる変更の種類を示します。 サポートされている値は `created`、`updated`、`deleted` です。 コンマ区切りのリストを使用して複数値を結合できます。<br><br>メモ: ドライブ ルート項目の通知は `updated` changeType のみに対応しています。 ユーザーとグループの通知は`updated` と `deleted` changeType に対応しています。|
| notificationUrl | 文字列 | 必須。 通知を受信するエンドポイントの URL。 この URL は必ず HTTPS プロトコルを使用する必要があります。 |
| リソース | 文字列 | 必須。 変更の監視対象となるリソースを指定します。 ベース URL (`https://graph.microsoft.com/v1.0/`) は含めないでください。 |
| expirationDateTime | [dateTime](http://tools.ietf.org/html/rfc3339) | 必須。 webhook サブスクリプションの有効期限が切れる日時を指定します。 時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。  サポートされているサブスクリプションの最長時間については、次の表をご覧ください。 |
| clientState | 文字列 | 省略可能。 各通知内のサービスによって送信される `clientState` プロパティの値を指定します。 最大の長さは 128 文字です。 クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。 |
| ID | 文字列 | サブスクリプションの一意の識別子です。読み取り専用です。 |
| applicationId | 文字列 | サブスクリプションを作成するために使用するアプリケーションの識別子です。 読み取り専用。 |
| creatorId | 文字列 | サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子です。 アプリケーションがサブスクリプションを作成するのに委任されたアクセス許可を使用した場合、このフィールドには、代理でアプリケーションが呼び出したサインイン中のユーザーの ID が含まれます。 アプリケーションは、アプリケーションのアクセス許可を使用した場合、このフィールドには、そのアプリケーションに対応するサービス プリンシパルの ID が含まれます。 読み取り専用。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>リソースの種類別のサブスクリプションの最大の長さ

| リソース            | 最大有効期限  |
|:--------------------|:-------------------------|
| メール                | 4230 分 (3 日間で)    |
| カレンダー            | 4230 分 (3 日間で)    |
| 連絡先            | 4230 分 (3 日間で)    |
| グループ会話 | 4230 分 (3 日間で)    |
| ドライブ ルート項目    | 4230 分 (3 日間で)    |

> **注意:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。 後になされる最大値を超えるサブスクリプションの作成や更新の要求は失敗します。

## <a name="relationships"></a>リレーションシップ

なし

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
| [サブスクリプションを作成](../api/subscription_post_subscriptions.md) | [サブスクリプション](subscription.md) | Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。 |
| [サブスクリプションを更新](../api/subscription_update.md) | [サブスクリプション](subscription.md) | 有効期限を更新することにより、サブスクリプションを更新します。 |
| [サブスクリプションをリスト](../api/subscription_list.md) | [サブスクリプション](subscription.md) | アクティブなサブスクリプションの一覧を表示します。 |
| [サブスクリプションを取得する](../api/subscription_get.md) | [サブスクリプション](subscription.md) | サブスクリプション オブジェクトのプロパティと関係を読み取ります。 |
| [サブスクリプションの削除](../api/subscription_delete.md) | なし |サブスクリプション オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
