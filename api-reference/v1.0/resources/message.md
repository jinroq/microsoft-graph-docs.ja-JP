---
title: メッセージ リソースの種類
description: mailFolder のメッセージ。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3f3a84e91cdfb20eacf764d5363ebc5fb3987dff
ms.sourcegitcommit: 00959f992b9b77c98ec1fe2f185cc7fd098ab24b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36426399"
---
# <a name="message-resource-type"></a>メッセージ リソースの種類

mailFolder のメッセージ。

Exchange Online メールボックスから送信される 1 つの電子メール メッセージのための **toRecipients**、**ccRecipients**、および **bccRecipients** プロパティに含まれる受信者の最大合計数は 500 です。 詳細については、「[送信の制限](https://docs.microsoft.com/ja-JP/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)」を参照してください。

このリソースは以下をサポートしています。

- カスタム インターネット メッセージ ヘッダーとして独自のデータを追加します。 メッセージの作成時にのみカスタム ヘッダーを追加し、ヘッダーに "x-" で始まる名前を付けます。 メッセージが送信された後ではヘッダーを変更することはできません。 メッセージのヘッダーを取得するには、[get message](../api/message-get.md) パラメーターで `$select` クエリ パラメーターを適用します。
- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)を受信します。
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
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|メッセージの BCC 受信者。|
|body|[itemBody](itembody.md)|メッセージの本文。 HTML 形式またはテキスト形式にできます。 [メッセージ本文での安全な HTML](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned) に関する情報を参照してください。|
|bodyPreview|String|メッセージ本文の最初の 255 文字。テキスト形式です。|
|categories|String collection|メッセージに関連付けられたカテゴリ。|
|ccRecipients|[recipient](recipient.md) collection|メッセージの CC 受信者。|
|changeKey|String|メッセージのバージョン。|
|conversationId|String|電子メールが属している会話の ID。|
|createdDateTime|DateTimeOffset|メッセージが作成された日時。|
|flag|[followUpFlag](followupflag.md)|メッセージのステータス、開始日、期限、または完了日を示すフラグ値。|
|from|[recipient](recipient.md)|メッセージのメールボックス所有者と送信者。 この値は、実際に使用されているメールボックスに対応している必要があります。 メッセージの[from プロパティと sender プロパティの設定](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)に関する詳細情報を参照してください。|
|hasAttachments|ブール値|メッセージに添付ファイルがあるかどうかを示します。このプロパティにはインライン添付ファイルが含まれていません。このためメッセージにインライン添付ファイルのみが含まれている場合、このプロパティは false です。インライン添付ファイルが存在するかどうかを確認するには、**body** プロパティを解析して `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">` などの `src` 属性を探します。|
|id|String|メッセージの一意識別子 (メッセージが移動または変更された場合、この値は変更される可能性があることに注意)|
|importance|importance| メッセージの重要度: `Low`、`Normal`、`High`。|
|inferenceClassification | inferenceClassificationType | 推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類。 使用可能な値: `focused`、`other`。 |
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) コレクション | [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) で定義されている一連のメッセージ ヘッダーです。 これには、メッセージが辿った送信者から受信者へのネットワーク パスを示すメッセージ ヘッダーが含まれています。 また、メッセージのアプリ データを保持するカスタム メッセージ ヘッダーも含めることができます。 <br><br> `$select` クエリ オプションの適用時にのみ、返されます。 読み取り専用です。 |
|internetMessageId |String |[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 |
|isDeliveryReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|isDraft|Boolean|メッセージが下書きかどうかを示します。メッセージがまだ送信されていなければ下書きです。|
|isRead|Boolean|メッセージが開封されたかどうかを示します。|
|isReadReceiptRequested|Boolean|メッセージの開封確認メッセージが要求されているかどうかを示します。|
|lastModifiedDateTime|DateTimeOffset|メッセージが最後に変更された日時。|
|parentFolderId|String|メッセージの親 mailFolder の一意識別子。|
|receivedDateTime|DateTimeOffset|メッセージが受信された日時です。|
|replyTo|[recipient](recipient.md) collection|返信時に使用される電子メール アドレス。|
|sender|[recipient](recipient.md)|メッセージを生成するために実際に使用されるアカウント。 ほとんどの場合、この値は **from** プロパティと同じです。 
  [共有メールボックス](https://docs.microsoft.com/ja-JP/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信するとき、またはメッセージを [delegate](https://support.office.com/ja-JP/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) として送信するときには、このプロパティに異なる値を設定できます。 いずれの場合でも、この値は、実際に使用されているメールボックスに対応している必要があります。 メッセージの[from プロパティと sender プロパティの設定](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)に関する詳細情報を参照してください。|
|sentDateTime|DateTimeOffset|メッセージが送信された日時。|
|subject|String|メッセージの件名。|
|toRecipients|[recipient](recipient.md) collection|メッセージの宛先。|
|uniqueBody|[itemBody](itembody.md)|現在のメッセージに一意であるメッセージの本文の一部。**uniqueBody** は、既定で返されませんが、特定のメッセージのために `?$select=uniqueBody` クエリを使用して取得することができます。HTML 形式またはテキスト形式にできます。|
|webLink|String|Outlook Web App でメッセージを開く URL。<br><br>URL の末尾に ispopout 引数を付加して、メッセージの表示方法を変更できます。ispopout が存在しない、または 1 に設定されている場合は、メッセージがポップアウト ウィンドウに表示されます。ispopout が 0 に設定されている場合、ブラウザーの Outlook Web App レビュー ウィンドウにメッセージが表示されます。<br><br>Outlook Web App のメールボックスにログインしている場合、ブラウザーでメッセージが開きます。まだブラウザーでログインしていない場合、ログインするように求められます。<br><br>この URL には、iFrame 内からアクセスできます。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md) コレクション|メッセージの [fileAttachment](fileattachment.md) 添付ファイルと [itemAttachment](itemattachment.md) 添付ファイル。|
|extensions|[extension](extension.md) コレクション|メッセージに対して定義されているオープン拡張機能のコレクションです。 Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| メッセージに対して定義された、複数値の拡張プロパティのコレクション。 Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| メッセージに対して定義された、単一値の拡張プロパティのコレクションです。 Null 許容型。|

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
    "multiValueExtendedProperties",

    "internetMessageHeaders"
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
