# <a name="mailfolder-resource-type"></a>mailFolder リソースの種類

受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。

このリソースでは、[デルタ](../api/mailfolder_delta.md)関数を用意すれば、増分の追加、削除、更新を追跡するために[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。

**既知のフォルダー名**

Outlook では、既定でユーザー用の特定のフォルダーを作成します。 対応するフォルダーの **id** 値を使用する代わりに、便利なことに、これらのフォルダーにアクセスするときに、次の表から既知のフォルダー名を使用できます。 たとえば、次のクエリで、既知の名前を使用して、[下書き] フォルダーを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

既知の名前は、ユーザーのメールボックスのロケールに関係なく機能します。そのため、上記のクエリは、命名方法に関わらず、常にユーザーの [下書き] フォルダーを返します。

| 既知のフォルダー名 | 説明 |
|:-----------------------|:------------|
| archive | archive フォルダーのメッセージは、"ワンクリックでアーカイブ" (クイックアーカイブ) 機能をサポートしている Outlook クライアントでこの機能を使用すると送信されます。 **注:** これは Exchange Online のアーカイブ メールボックス機能とは異なります。 |
| clutter | [低優先メール] フォルダーの優先順位の低いメッセージは、低優先メール機能を使用すると移動されます。 |
| conflicts | メールボックスにある競合アイテムを含むフォルダーです。 |
| conversationhistory |  (Skype がこの動作を実行するように構成されている場合) Skype が IM での会話を保存するフォルダーです。 |
| deleteditems | フォルダーのアイテムは削除時に移動されます。 |
| drafts | 未送信のメッセージを含むフォルダーです。 |
| inbox | 受信トレイのフォルダーです。 |
| junkemail | 迷惑メールのフォルダーです。 |
| localfailures | ローカル クライアント上に存在するが、サーバーにアップロードできなかったアイテムを含むフォルダーです。 |
| msgfolderroot | "インフォメーション ストアの最上位" のフォルダーです。 このフォルダーは、受信トレイなど、通常のメール クライアントで表示されているフォルダーの親フォルダーです。 |
| outbox | 送信トレイのフォルダーです。 |
| recoverableitemsdeletions | 論理的に削除されたアイテムを含むフォルダーです。つまり、[削除済みアイテム]フォルダーから、または  Outlook で Shift キーを押しながら Delete キーを押して削除されたアイテムです。 このフォルダーは Outlook のメール クライアントには表示されませんが、エンドユーザーは、Outlook または Outlook on the web の **[サーバーから削除済みアイテムを復元] ** 機能を使用して、このフォルダーにアクセスできます。 |
| scheduled | iOS 版 Outlook のスケジュール機能を使用して受信トレイに再表示されるようにスケジュールされているメッセージを含むフォルダーです。 |
| searchfolders | ユーザーのメールボックスで定義されているすべての検索フォルダーの親フォルダーです。 |
| sentitems | 送信済みアイテムのフォルダーです。 |
| serverfailures | サーバー上に存在するが、ローカル クライアントに同期できなかったアイテムを含むフォルダーです。 |
| syncissues | Outlook で作成された同期ログを含むフォルダーです。 |

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
|[mailFolder の取得](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MailFolder の作成](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。|
|[childFolders を一覧表示する](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md) コレクション| 指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。|
|[メッセージの作成](../api/mailfolder_post_messages.md) |[メッセージ](message.md)| メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。|
|[メッセージのリスト](../api/mailfolder_list_messages.md) |[Message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。|
|[更新する](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|指定した mailFolder オブジェクトを更新します。 |
|[削除](../api/mailfolder_delete.md) | なし |指定した mailFolder オブジェクトを削除します。 |
|[コピー](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder にコピーします。|
|[デルタ](../api/mailfolder_delta.md)|[mailFolder](mailfolder.md) コレクション|ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。|
|[移動](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder に移動します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ mailFolder の取得](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。`$expand` |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | 新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ mailFolder の取得](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | を使用して、複数値の拡張プロパティを含む mailFolder を取得します。`$expand` |

## <a name="properties"></a>プロパティ

| プロパティ | タイプ | 説明 |
|:---------|:-----|:------------|
|childFolderCount|Int32|現在の mailFolder の直下の子 mailFolder の数。|
|displayName|文字列|mailFolder の表示名。|
|id|文字列|MailFolder の一意の識別子です。|
|parentFolderId|文字列|mailFolder の親 mailFolder の一意識別子。|
|totalItemCount|Int32|mailFolder に含まれるアイテムの数|
|unreadItemCount|Int32|mailFolder 内で未読としてマークされているアイテムの数。|

**アイテム数を効率的に取得する**

フォルダーの `TotalItemCount` プロパティと `UnreadItemCount` プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。
これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook のメール フォルダーには複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メール アイテムとは異なる会議出席依頼アイテムを入れることができます。 `TotalItemCount`  `UnreadItemCount` には、アイテムの種類に関係なく、[メール] フォルダー内のアイテムが含まれます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) コレクション|mailFolder 内の子フォルダーのコレクション。|
|messageRules | [messageRule](messagerule.md) コレクション | ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。 |
|messages|[Message](message.md) コレクション|mailFolder 内のメッセージのコレクション。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](../../../concepts/delta_query_overview.md)
- [フォルダー内のメッセージへの増分の変更を取得する](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
