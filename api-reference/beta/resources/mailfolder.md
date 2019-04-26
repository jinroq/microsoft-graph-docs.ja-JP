---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 294f2a9a6b4775ad30165352dec5520fb0efa804
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342774"
---
# <a name="mailfolder-resource-type"></a>mailFolder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。

このリソースでは、[デルタ](../api/mailfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。

**既知のフォルダー名**

Outlook では、既定でユーザー用の特定のフォルダーを作成します。 このようなフォルダーにアクセスする場合は、対応するフォルダー **id**値を使用する代わりに、以下の表にある、既知のフォルダー名を使用することもできます。 たとえば、次のクエリを使用して、既知の名前を使用して [下書き] フォルダーを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

既知の名前は、ユーザーのメールボックスのロケールに関係なく動作するので、上記のクエリは、名前の指定に関係なく、常にユーザーの [下書き] フォルダーを返します。

| 既知のフォルダー名 | 説明 |
|:-----------------------|:------------|
| ・ | アーカイブフォルダーのメッセージは、それをサポートする Outlook クライアントで One_Click アーカイブ機能を使用するときに送信されます。 **注:** これは、Exchange online のアーカイブメールボックス機能と同じではありません。 |
| 整頓 | 低優先メール機能フォルダー低優先度のメッセージは、低優先メール機能を使用している場合に移動されます。 |
| 解消 | メールボックス内の競合するアイテムを含むフォルダー。 |
| conversationhistory | skype が IM 会話を保存するフォルダー (skype が設定されている場合)。 |
| deleteditems | フォルダーアイテムは、削除されたときに移動されます。 |
| 未公開 | 未送信メッセージを含むフォルダー。 |
| ボックス | 受信トレイフォルダー。 |
| junkemail | 迷惑メールフォルダー。 |
| localfailures | ローカルクライアント上に存在するが、サーバーにアップロードできないアイテムを含むフォルダー。 |
| msgfolderroot | "インフォメーションストアのトップ" フォルダー このフォルダーは、受信トレイなど、通常のメールクライアントに表示されるフォルダーの親フォルダーです。 |
| 送信トレイ | 送信トレイフォルダー。 |
| recoverableitemsdeletions | 削除済みアイテムフォルダーから削除された、または Outlook で shift + del キーを押して削除されたアイテムを含むフォルダー。 このフォルダーは、outlook 電子メールクライアントでは表示されませんが、エンドユーザーは、outlook または web 上の outlook の [**サーバーからの削除済みアイテムを復元**する] 機能を使用して操作できます。 |
| スケジュール済み | iOS 版 Outlook のスケジュール機能を使用して、受信トレイに再表示するようにスケジュールされたメッセージを含むフォルダー。 |
| searchfolders | ユーザーのメールボックスに定義されているすべての検索フォルダーの親フォルダーです。 |
| sentitems | 送信済みアイテムフォルダー。 |
| serverfailures | サーバー上に存在するが、ローカルクライアントに同期できなかったアイテムを含むフォルダー。 |
| syncissues 問題 | Outlook によって作成された同期ログが格納されているフォルダー。 |

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
|[mailFolder の取得](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MailFolder の作成](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。|
|[childFolders を一覧表示する](../api/mailfolder-list-childfolders.md) |[mailFolder](mailfolder.md) コレクション| 指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。|
|[メッセージの作成](../api/mailfolder-post-messages.md) |[message](message.md)| メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。|
|[List messages](../api/mailfolder-list-messages.md) |[message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。|
|[更新する](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|指定した mailFolder オブジェクトを更新します。 |
|[削除](../api/mailfolder-delete.md) | なし |指定した mailFolder オブジェクトを削除します。 |
|[コピー](../api/mailfolder-copy.md)|[mailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder にコピーします。|
|[delta](../api/mailfolder-delta.md)|[mailFolder](mailfolder.md) コレクション|ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。|
|[move](../api/mailfolder-move.md)|[mailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder に移動します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |新規または既存の mailFolder に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ mailFolder の取得](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む mailFolder を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | 新規または既存の mailFolder の 1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ mailFolder の取得](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | `$expand` を使用して、複数値の拡張プロパティを含む mailFolder を取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
|childFolderCount|Int32|現在の mailFolder の直下の子 mailFolder の数。|
|displayName|文字列|mailFolder の表示名。|
|id|String|mailfolder の一意の識別子。|
|parentFolderId|String|mailFolder の親 mailFolder の一意識別子。|
|totalItemCount|Int32|mailFolder に含まれるアイテムの数|
|unreadItemCount|Int32|mailFolder 内で未読としてマークされているアイテムの数。|
|wellKnownName|String|フォルダーの既知のフォルダー名。 指定できる値は、上記のとおりです。 このプロパティは、Outlook によって作成された既定のフォルダーに対してのみ設定されます。 その他のフォルダーの場合、このプロパティは**null**になります。|

**アイテム数の効率的な取得**

フォルダー `TotalItemCount`の`UnreadItemCount`プロパティとプロパティを使用すると、フォルダー内の閲覧アイテムの数を簡単に計算できます。
これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook のメールフォルダーには、複数の種類のアイテムを含めることができます。たとえば、受信トレイには、メールアイテムとは異なる会議出席依頼アイテムを含めることができます。 `TotalItemCount`アイテム`UnreadItemCount`の種類に関係なく、メールフォルダーにアイテムを追加します。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) コレクション|mailFolder 内の子フォルダーのコレクション。|
|messageRules | [messageRule](messagerule.md) コレクション | ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。 |
|messages|[Message](message.md) collection|mailFolder 内のメッセージのコレクション。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

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
  "wellKnownName": "string",
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
