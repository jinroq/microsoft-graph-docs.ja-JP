# <a name="mailfolder-resource-type"></a>mailFolder リソースの種類

受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。

Outlook では、既定でユーザー用の特定のフォルダーを作成します。 対応するフォルダーの **id** 値の代わりに、便宜のために、既知のフォルダー名 (`ArchiveRoot`、`ConversationHistory`、`DeletedItems`、`Drafts`、`Inbox`、`JunkEmail`、`Outbox`、`SentItems`) を使用して、**mailFolder** コレクションのフォルダーにアクセスすることができます。

このリソースでは、[デルタ](../api/mailfolder_delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用できます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[mailFolder の取得](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MailFolder の作成](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。|
|[childFolders を一覧表示する](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md) コレクション| 指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。|
|[メッセージの作成](../api/mailfolder_post_messages.md) |[Message](message.md)| メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。|
|[List messages](../api/mailfolder_list_messages.md) |[Message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。|
|[更新する](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|指定した mailFolder オブジェクトを更新します。 |
|[削除](../api/mailfolder_delete.md) | なし |指定した mailFolder オブジェクトを削除します。 |
|[コピー](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder にコピーします。|
|[delta](../api/mailfolder_delta.md)|[mailFolder](mailfolder.md) コレクション|ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。|
|[move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder に移動します。|
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ mailFolder の取得](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | 新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ mailFolder の取得](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | `$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|childFolderCount|Int32|現在の mailFolder の直下の子 mailFolder の数。|
|displayName|String|mailFolder の表示名。|
|id|String|mailFolder の一意識別子。次の既知の名前を使用して対応するフォルダーにアクセスできます。Inbox、Drafts、SentItems、DeletedItems。|
|parentFolderId|String|mailFolder の親 mailFolder の一意識別子。|
|totalItemCount|Int32|mailFolder に含まれるアイテムの数|
|unreadItemCount|Int32|mailFolder 内で未読としてマークされているアイテムの数。|

**アイテム数を効率的に取得する**

フォルダーの TotalItemCount プロパティと UnreadItemCount プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
Outlook 内の MailFolder には、複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メール アイテムとは異なる会議出席依頼アイテムを入れることができます。TotalItemCount と UnreadItemCount には、アイテムの種類に関係なく、mailFolder 内のアイテムが含まれます。


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|childFolders|[MailFolder](mailfolder.md) コレクション|mailFolder 内の子フォルダーのコレクション。|
|messageRules | [messageRule](messagerule.md) コレクション | ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。 | 
|messages|[Message](message.md) コレクション|mailFolder 内のメッセージのコレクション。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules", 
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
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
