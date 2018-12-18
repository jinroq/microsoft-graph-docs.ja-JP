---
title: post リソース タイプ
description: ConverstaionThread エンティティ内の個々 の投稿アイテムを表します。
author: dkershaw10
ms.openlocfilehash: 6030bd5ef3c59edbad9712b549531a193b808b14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363719"
---
# <a name="post-resource-type"></a>post リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ConverstaionThread](conversationthread.md)エンティティ内の個々 の投稿アイテムを表します。

投稿を明示的に作成できなくても、次のいずれかの方法で投稿を作成できます。

* [既存の投稿に返信する](../api/post-reply.md) 
* [既存のスレッドに返信する](../api/conversationthread-reply.md) 
* [新しい会話にスレッドを作成する](../api/group-post-threads.md)
* [新しい会話を作成する](../api/group-post-conversations.md)

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|投稿の内容です。これが既定のプロパティです。このプロパティを null にすることができます。|
|categories|String コレクション|投稿に関連付けられたカテゴリ。 各カテゴリは、ユーザーが定義されている[outlookCategory](outlookcategory.md)の**表示名**のプロパティに対応します。|
|changeKey|String|投稿のバージョンを識別します。投稿を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|conversationId|String|会話の固有 ID です。読み取り専用。|
|conversationThreadId|String|会話スレッドの固有 ID です。読み取り専用。|
|createdDateTime|DateTimeOffset|投稿の作成時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|from|[recipient](recipient.md)|代理人アクセスのシナリオで使用されます。他のユーザーの代わりにメッセージを投稿したユーザーを示します。これが既定のプロパティです。|
|hasAttachments|ブール型|投稿の添付ファイルが 1 つ以上あるかどうかを示します。これが既定のプロパティです。|
|id|String| 読み取り専用。|
|importance | String | グループのポストの重要性: `low`、 `normal`、 `high`。 |
|lastModifiedDateTime|DateTimeOffset|投稿が最後に修正された日時を指定します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|newParticipants|[recipient](recipient.md) collection|この投稿の一部としてスレッドに追加された会話の参加者です。|
|receivedDateTime|DateTimeOffset|投稿の受信時刻を示します。DateTimeOffset 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|sender|[recipient](recipient.md)|送信者のアドレスが含まれます。送信者が指定されていない場合、送信者の値は認証済みユーザーのアドレスと見なされます。これが既定のプロパティです。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|attachments|[Attachment](attachment.md) コレクション|投稿の[fileAttachment](fileattachment.md)、 [itemAttachment](itemattachment.md)、および[referenceAttachment](referenceattachment.md)の添付ファイルのコレクションです。 読み取り専用です。 Null 許容型。|
|extensions|[Extension](extension.md) コレクション|投稿に対して定義されているオープン拡張機能のコレクション。読み取り専用。Null 許容型。|
|inReplyTo|[Post](post.md)|[ConversationThread](conversationthread.md)でへこの投稿の返信は、以前の投稿です。 読み取り専用。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| その投稿用に定義された、複数値拡張プロパティのコレクションです。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| その投稿用に定義された、単一値拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[List posts](../api/conversationthread-list-posts.md) | [post](post.md) |指定したスレッドの投稿を取得します。 |
|[Get post](../api/post-get.md) | [post](post.md) |指定したスレッド内の投稿のプロパティと関係を取得します。|
|[Reply](../api/post-reply.md)|なし|グループ会話の投稿に返信して、指定されたスレッドに新しい投稿を追加します。|
|[Forward](../api/post-forward.md)|なし|受信者に投稿を転送します。|
|**添付ファイル**| | |
|[添付ファイルを一覧表示する](../api/post-list-attachments.md) |[attachment](attachment.md) コレクション| 投稿のすべての添付ファイルを取得します。|
|[添付ファイルを追加する](../api/post-post-attachments.md) |[attachment](attachment.md)| 投稿に添付ファイルを追加します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |新規または既存の投稿に、ひとつまたは複数の単一値の拡張プロパティを作成します。   |
|[Get post with single-value extended property](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む投稿を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | 新規または既存の投稿に、ひとつまたは複数の複数値の拡張プロパティを作成します。  |
|[Get post with multi-value extended property](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | `$expand` を使用して、複数値の拡張プロパティを含む投稿を取得します。 |

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->