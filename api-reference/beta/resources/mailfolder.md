---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1cd48c866ea6384aa18631732065380e898b8bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642696"
---
# <a name="mailfolder-resource-type"></a>mailFolder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。

このリソースでは、[デルタ](../api/mailfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。

**既知のフォルダー名**

Outlook では、既定でユーザー用の特定のフォルダーを作成します。 対応するフォルダーの**id**値を使用して、利便性のため、代わりにこれらのフォルダーにアクセスするときに既知のフォルダー名を次の表からを使用できます。 たとえば、次のクエリを使用して、既知の名前を使用して、[下書き] フォルダーを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

既知の名前は、上記のクエリは、常に付けの方法に関係なく、ユーザーの [下書き] フォルダーを返しますので、ユーザーのメールボックスのロケールに関係なく動作します。

| 既知のフォルダー名 | 説明 |
|:-----------------------|:------------|
| アーカイブ | アーカイブ フォルダーのメッセージは、サポートしている Outlook クライアントで One_Click のアーカイブ機能を使用する場合に送信されます。 **注:** これは Exchange のメールボックスのアーカイブの機能は、オンラインの場合と同じです。 |
| 散乱 | 整理フォルダーの優先順位の低いメッセージは、整理機能を使用するときに移動されます。 |
| 競合 | メールボックスにある競合アイテムを含むフォルダーです。 |
| conversationhistory | (これを行うには、Skype が構成されている) 場合に、Skype が IM の会話を保存するフォルダーです。 |
| deleteditems | フォルダーのアイテムは、削除するときに移動されます。 |
| 下書き | 未送信のメッセージを格納するフォルダー。 |
| [受信トレイ] | [受信トレイ] フォルダーです。 |
| junkemail | 迷惑メールのフォルダーです。 |
| localfailures | ローカル クライアント上に存在するが、サーバーにアップロードできませんでしたアイテムを含むフォルダーです。 |
| msgfolderroot | 「インフォメーション ストアの最上位」のフォルダーです。 このフォルダーは、受信トレイなど、通常のメール クライアントで表示されているフォルダーの親フォルダーです。 |
| [送信トレイ] します。 | [送信トレイ] フォルダーです。 |
| recoverableitemsdeletions | ソフト削除済みアイテムを含むフォルダー: 削除済みアイテム フォルダーから、または shift キーを押して削除 + では、Outlook を削除します。 このフォルダーが、Outlook 電子メール クライアントに表示されないが、エンド ・ ユーザーを操作できます Outlook または Outlook web 上で**サーバーから削除済みアイテムの回復**機能を使用します。 |
| スケジュール済み | IOS は、Outlook のスケジュール機能を使用して受信トレイに表示されるようにスケジュールされているメッセージを含むフォルダーです。 |
| 使用して | ユーザーのメールボックスで定義されているすべての検索フォルダーの親フォルダーです。 |
| 送信済みアイテム | 送信済みアイテム フォルダーです。 |
| serverfailures | サーバー上に存在するが、ローカル クライアントを同期できませんでしたアイテムを含むフォルダーです。 |
| syncissues | Outlook で作成された同期ログを格納するフォルダー。 |

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
|displayName|String|mailFolder の表示名。|
|id|String|MailFolder の一意の識別子です。|
|parentFolderId|String|mailFolder の親 mailFolder の一意識別子。|
|totalItemCount|Int32|mailFolder に含まれるアイテムの数|
|unreadItemCount|Int32|mailFolder 内で未読としてマークされているアイテムの数。|
|wellKnownName|String|フォルダーの既知のフォルダーの名前です。 可能な値は、上記に一覧表示されます。 Outlook で作成された既定のフォルダーには、このプロパティは設定のみです。 その他のフォルダーでは、このプロパティは**null**です。|

**アイテム数を効率的に取得する**

`TotalItemCount`と`UnreadItemCount`フォルダーのプロパティを使用すると、簡単にフォルダー内のアイテムの読み取りの数を計算します。
これにより、大幅な遅延が発生する可能性がある次のようなクエリを回避できます。

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook のメール フォルダーにアイテムの 1 つ以上の種類を含めることができます、受信トレイを含めることができますたとえば、会議出席依頼アイテムがメール アイテムとは異なる。 `TotalItemCount``UnreadItemCount`の項目の種類に関係なく、[メール] フォルダーにアイテムが含まれます。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) コレクション|mailFolder 内の子フォルダーのコレクション。|
|messageRules | [messageRule](messagerule.md) コレクション | ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。 |
|messages|[Message](message.md) コレクション|mailFolder 内のメッセージのコレクション。|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/mailfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
