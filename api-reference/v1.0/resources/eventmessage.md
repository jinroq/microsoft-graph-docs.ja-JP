# <a name="eventmessage-resource-type"></a>eventMessage リソースの種類

会議出席依頼、会議中止メッセージ、会議承諾メッセージ、会議仮承諾メッセージ、または会議辞退メッセージを表すメッセージです。

通常、EventMessage は、イベント開催者が会議を作成した結果、または参加者が会議出席依頼に応答した結果として、受信トレイ フォルダーに届けられます。イベント メッセージには Message と同様の方法で対処しますが、次の表に示すようなわずかな違いがあります。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[eventMessage の取得](../api/eventmessage_get.md) | [eventMessage](eventmessage.md) |eventMessage オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/eventmessage_update.md) | [eventMessage](eventmessage.md)  |eventMessage オブジェクトを更新します。 |
|[削除](../api/message_delete.md) | なし |eventMessage オブジェクトを削除します。 |
|[コピー](../api/message_copy.md)|[Message](message.md)|メッセージをフォルダーにコピーします。|
|[createForward](../api/message_createforward.md)|[Message](message.md)|転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[createReply](../api/message_createreply.md)|[Message](message.md)|返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[createReplyAll](../api/message_createreplyall.md)|[Message](message.md)|全員に返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message_update.md)または[送信](../api/message_send.md)できます。|
|[forward](../api/message_forward.md)|なし|メッセージを転送します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[移動](../api/message_move.md)|[Message](message.md)|メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。|
|[返信](../api/message_reply.md)|なし|メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[replyAll](../api/message_replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message_send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/eventmessage_list_attachments.md) |[Attachment](attachment.md) コレクション| eventMessage のすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/eventmessage_post_attachments.md) |[Attachment](attachment.md)| 添付ファイル コレクションへの投稿により、eventMessage に新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを 1 つまたは複数取得します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[eventMessage](eventMessage.md)  |新規または既存の eventMessage に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ eventMessage の取得](../api/singlevaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む eventMessage を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [eventMessage](eventMessage.md) | 新規または既存の eventMessage に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ eventMessage の取得](../api/multivaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | `$expand` を使用して、複数値の拡張プロパティを含む eventMessage を取得します。 |


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。|
|categories|String collection|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。|
|hasAttachments|Boolean|メッセージに添付ファイルがあるかどうかを示します。|
|id|String||
|importance|String| メッセージの重要度: `Low`、`Normal`、`High`。|
|internetMessageId |String |[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 |
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|meetingMessageType|String| イベント メッセージの種類: `None`、`MeetingRequest`、`MeetingCancelled``MeetingAccepted``MeetingTenativelyAccepted``MeetingDeclined`。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに特有のメッセージの本文の一部。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) コレクション| 読み取り専用。Null 許容型。|
|イベント|[Event](event.md)| イベント メッセージに関連付けられたイベント。参加者または部屋リソースの前提は、会議出席依頼イベント メッセージが届いたときにイベントを含む予定表を自動的に更新するようにカレンダー アテンダントが設定されていることです。ナビゲーション プロパティ。読み取り専用。|
|extensions|[Extension](extension.md) コレクション|eventMessage に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| eventMessage に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| eventMessage に対して定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventmessage"
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
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "meetingMessageType": "String",
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
