---
title: メッセージ リソースの種類
description: mailFolder のメッセージ。
author: angelgolfer-ms
ms.openlocfilehash: a77a50835dcba41555fa646c94c66d05b15e3e48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310291"
---
# <a name="message-resource-type"></a>メッセージ リソースの種類

mailFolder のメッセージ。

このリソースは以下をサポートしています。

- カスタムのインターネット メッセージのヘッダーとして、独自のデータを追加しています。 メッセージを作成するときにのみ、カスタム ヘッダーを追加し、名前を付けます"x-"で始まります。 メッセージが送信されると、ヘッダーを変更することはできません。 メッセージのヘッダーを取得するには、適用、 `$select` 、[メッセージの取得](../api/message-get.md)操作のパラメーターのクエリを実行します。
- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティとしては、独自のデータを追加します。
- [変更通知](/graph/webhooks)にサブスクライブします。
- [デルタ](../api/message-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[List messages](../api/user-list-messages.md) |[message](message.md) コレクション | サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。 |
|[メッセージの作成](../api/user-post-messages.md) | [message](message.md) | 新しいメッセージの下書きを[作成](../api/user-post-messages.md#request-1)します。 |
|[メッセージの取得](../api/message-get.md) | [message](message.md) |message オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/message-update.md) | [message](message.md) |メッセージ オブジェクトを更新します。|
|[削除](../api/message-delete.md) | なし |メッセージ オブジェクトを削除します。 |
|[コピー](../api/message-copy.md)|[Message](message.md)|メッセージをフォルダーにコピーします。|
|[createForward](../api/message-createforward.md)|[Message](message.md)|転送メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[createReply](../api/message-createreply.md)|[Message](message.md)|返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)|全員に返信メッセージの下書きを作成します。その後、下書きを[更新](../api/message-update.md)または[送信](../api/message-send.md)できます。|
|[delta](../api/message-delta.md)|[message](message.md) コレクション| 指定したフォルダーで追加、削除、更新されたメッセージのセットを取得します。|
|[forward](../api/message-forward.md)|なし|メッセージを転送します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[移動](../api/message-move.md)|[Message](message.md)|メッセージをフォルダーに移動します。これにより、宛先フォルダーにメッセージの新しいコピーが作成されます。|
|[返信](../api/message-reply.md)|なし|メッセージの送信者に返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[replyAll](../api/message-replyall.md)|なし|メッセージの受信者すべてに返信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|[送信](../api/message-send.md)|なし|以前に作成したメッセージの下書きを送信します。その後、メッセージは送信済みアイテム フォルダーに保存されます。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/message-list-attachments.md) |[Attachment](attachment.md) コレクション| メッセージのすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/message-post-attachments.md) |[Attachment](attachment.md)| 添付ファイル コレクションへの投稿により、メッセージに新しい添付ファイルを追加します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、リソースの新規または既存のインスタンスのカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 名前や完全修飾名によって識別されたオープン拡張機能オブジェクトを取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[message](message.md)  |新規または既存のメッセージに、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つメッセージの取得](../api/singlevaluelegacyextendedproperty-get.md)  | [message](message.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含むメッセージを取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [message](message.md) | 新規または既存のメッセージに、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つメッセージの取得](../api/multivaluelegacyextendedproperty-get.md)  | [message](message.md) | `$expand` を使用して、複数値の拡張プロパティを含むメッセージを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。 Html 形式またはテキスト形式でことができます。 [メッセージの本文内の安全な HTML](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned)をお探しです。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。テキスト形式です。|
|categories|String コレクション|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|flag|[followupFlag](followupflag.md)|メッセージのステータス、開始日、期限、または完了日を示すフラグ値。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。 値は、使用される実際のメールボックスに対応する必要があります。 について[の設定からとセンダーのプロパティ](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)のメッセージです。|
|hasAttachments|ブール値|メッセージに添付ファイルがあるかどうかを示します。このプロパティにはインライン添付ファイルが含まれていません。このためメッセージにインライン添付ファイルのみが含まれている場合、このプロパティは false です。インライン添付ファイルが存在するかどうかを確認するには、**body** プロパティを解析して `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">` などの `src` 属性を探します。|
|id|String|メッセージの一意識別子 (メッセージが移動または変更された場合、この値は変更される可能性があることに注意)|
|importance|importance| メッセージの重要度: `Low`、`Normal`、`High`。|
|inferenceClassification | inferenceClassificationType | 推論の妥当性や重要度、または明示的なオーバーライドに基づいて、ユーザーに対するメッセージの分類です。 可能な値:`focused`または`other`。 |
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) コレクション | [RFC5322](https://www.ietf.org/rfc/rfc5322.txt)で定義されているメッセージ ヘッダーのコレクションです。 セットには、受信者に送信者からのメッセージを取得するネットワーク パスを示すメッセージのヘッダーが含まれています。 メッセージのアプリケーション データを保持するカスタム メッセージのヘッダーを含めることもできます。 |
|internetMessageId |String |[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 |
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|ブール型|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。 ほとんどの場合、この値は、 **from**プロパティと同じです。 [共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)、または[委任](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信するメッセージを送信するとき、別の値にこのプロパティを設定できます。 いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。 について[の設定からとセンダーのプロパティ](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)のメッセージです。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに一意であるメッセージの本文の一部。**uniqueBody** は、既定で返されませんが、特定のメッセージのために `?$select=uniqueBody` クエリを使用して取得することができます。HTML 形式またはテキスト形式にできます。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|メッセージの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイル。|
|extensions|[extension](extension.md) コレクション|メッセージに対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| メッセージに対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| メッセージに対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
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
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
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
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}

```

## <a name="see-also"></a>関連項目

- [メールボックス設定を取得する](../api/user-get-mailboxsettings.md) 
- [メールボックス設定を更新する](../api/user-update-mailboxsettings.md)
- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [フォルダー内のメッセージへの増分変更を取得する](/graph/delta-query-messages)
- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
