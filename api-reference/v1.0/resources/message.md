# <a name="message-resource-type"></a>メッセージ リソースの種類

mailFolder のメッセージ。

このリソースは以下をサポートしています。

- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/message_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[List messages](../api/user_list_messages.md) |[message](message.md) コレクション | サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。 |
|[メッセージの作成](../api/user_post_messages.md) | [message](message.md) | 新しいメッセージの下書きを[作成](../api/user_post_messages.md#request-1)します。 |
|[メッセージの取得](../api/message_get.md) | [message](message.md) |message オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/message_update.md) | [message](message.md) |メッセージ オブジェクトを更新します。|
|[削除](../api/message_delete.md) | なし |メッセージ オブジェクトを削除します。 |
|[コピー](../api/message_copy.md)|[Message](message.md)|メッセージをフォルダーにコピーします。|
|[createForward](../api/message_createforward.md)|[Message](message.md)|転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[createReply](../api/message_createreply.md)|[Message](message.md)|返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[createReplyAll](../api/message_createreplyall.md)|[Message](message.md)|全員に返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[delta](../api/message_delta.md)|[message](message.md) コレクション| 指定したフォルダーで追加、削除、更新されたメッセージのセットを取得します。|
|[forward](../api/message_forward.md)|なし|メッセージを転送します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[移動](../api/message_move.md)|[Message](message.md)|メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。|
|[返信](../api/message_reply.md)|なし|メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[replyAll](../api/message_replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message_send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/message_list_attachments.md) |[Attachment](attachment.md) コレクション| メッセージのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/message_post_attachments.md) |[Attachment](attachment.md)| 添付ファイル コレクションへの投稿により、メッセージに新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](../../../concepts/extensibility_schema_groups.md) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[message](message.md)  |新規または既存のメッセージに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つメッセージの取得](../api/singlevaluelegacyextendedproperty_get.md)  | [message](message.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含むメッセージを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [message](message.md) | 新規または既存のメッセージに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つメッセージの取得](../api/multivaluelegacyextendedproperty_get.md)  | [message](message.md) | `$expand` を使用して、複数値の拡張プロパティを含むメッセージを取得します。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。HTML 形式またはテキスト形式にできます。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。テキスト形式です。|
|categories|String collection|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。|
|hasAttachments|Boolean|メッセージに添付ファイルがあるかどうかを示します。このプロパティにはインライン添付ファイルが含まれていません。このためメッセージにインライン添付ファイルのみが含まれている場合、このプロパティは false です。インライン添付ファイルが存在するかどうかを確認するには、**body** プロパティを解析して `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">` などの `src` 属性を探します。|
|id|String|メッセージの一意識別子 (メッセージが移動または変更された場合、この値は変更される可能性があることに注意)|
|importance|String| メッセージの重要度: `Low`、`Normal`、`High`。|
|inferenceClassification | String | 推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。 |
|internetMessageId |String |[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 |
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに一意であるメッセージの本文の一部。**uniqueBody** は、既定で返されませんが、特定のメッセージのために `?$select=uniqueBody` クエリを使用して取得することができます。HTML 形式またはテキスト形式にできます。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|

**body プロパティからのスクリプトの削除**

メッセージ本文は、HTML またはテキストのいずれかにできます。本文が HTML の場合、既定では、**body** プロパティに組み込まれている安全ではない可能性がある HTML (たとえば、JavaScript など) が、本文の内容が REST 応答で返される前に削除されます。元の HTML コンテンツ全体を取得するには、次の HTTP 要求ヘッダーを含めます。
```
Prefer: outlook.allow-unsafe-html
```

**from プロパティと sender プロパティの設定**

メッセージが作成されるとき、ほとんどの場合には From プロパティと Sender プロパティは、同じサインイン ユーザーを示します。ただし、次のシナリオで説明されているように、どちらかが更新される場合は例外です。

- **from** プロパティは、Exchange 管理者がメールボックスの **sendAs** 権限を他のユーザーに割り当てた場合に変更できます。管理者は、Azure 管理ポータルでメールボックス所有者の**メールボックスのアクセス許可**を選択するか、Exchange 管理センターまたは Windows PowerShell Add-ADPermission コマンドレットを使用してこれを行えます。その後、プログラムを使用して、**from** プロパティを、対象メールボックスの **sendAs** 権限を持ついずれかのユーザーに自動的に設定できます。
- **sender** プロパティは、メールボックス所有者が 1 人以上のユーザーにそのメールボックスからメッセージを送信する権限を委任すると、変更できます。メールボックス所有者は、Outlook で委任できます。代理人がメールボックス所有者に代わってメッセージを送信する場合、**sender** プロパティは代理人のアカウントに設定され、**from** プロパティはメールボックス所有者のままになります。プログラムを使用して、**sender** プロパティを、対象メールボックスの委任権限を取得したユーザーに設定できます。

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|メッセージの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイル。|
|extensions|[extension](extension.md) コレクション|メッセージに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| メッセージに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| メッセージに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <a name="see-also"></a>関連項目

- [メールボックス設定を取得する](../api/user_get_mailboxsettings.md) 
- [メールボックス設定を更新する](../api/user_update_mailboxsettings.md)
- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](../../../concepts/delta_query_overview.md)
- [フォルダー内のメッセージへの増分変更を取得する](../../../concepts/delta_query_messages.md)
- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
