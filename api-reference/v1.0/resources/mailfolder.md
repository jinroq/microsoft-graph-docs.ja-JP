---
title: mailFolder リソースの種類
description: 受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dbcb35ad0b131f4e714acd7f178fbbb1109b913c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574027"
---
# <a name="mailfolder-resource-type"></a>mailFolder リソースの種類

受信トレイや下書きなどの、ユーザーのメールボックス内のメール フォルダーです。 メール フォルダーには、メッセージ、他の Outlook アイテム、子メール フォルダーを含めることができます。

このリソースは、[デルタ](../api/mailfolder-delta.md)関数を提供することによって、増分の追加、削除、および更新を追跡するための[デルタ クエリ](/graph/delta-query-overview)の使用をサポートしています。

**既知のフォルダー名**

Outlookは、デフォルトでユーザー用の特定のフォルダーを作成します。 対応するフォルダ**id**値を使用する代わりに、便宜上、これらのフォルダにアクセスするときに、下の表にある既知のフォルダ名を使用できます。 たとえば、次のクエリで、よく知られている名前を使用して[下書き]フォルダを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

既知の名前はユーザーのメールボックスのロケールに関係なく機能するため、上記のクエリでは名前の付け方にかかわらず常にユーザーの[下書き]フォルダーが返されます。

| 既知のフォルダー名 | 説明 |
|:-----------------------|:------------|
| アーカイブ | アーカイブ フォルダーのメッセージは、対応する Outlook クライアントで One_Click アーカイブ機能を使用するときに送信されます。 **注意:** これはExchange Onlineのアーカイブメールボックス機能と同じではありません。 |
| 低優先メール | [Clutter]機能を使用すると、clutterフォルダに優先順位の低いメッセージがに移動されます。 |
| 競合 | メールボックス内で競合するアイテムが含まれているフォルダ。 |
| conversationhistory | SkypeがIM会話を保存するフォルダ（Skypeがそうするように設定されている場合）。 |
| deleteditems | フォルダ項目は、削除されたときに移動されます。 |
| 下書き | 未送信メッセージが含まれているフォルダ。 |
| inbox | 受信トレイ フォルダー。 |
| junkemail | [迷惑メール] フォルダー。 |
| localfailures | ローカルクライアントに存在するがサーバーにアップロードできなかったアイテムを含むフォルダ。 |
| msgfolderroot | "Top of Information Store" フォルダ。 このフォルダは、受信トレイなど、通常のメールクライアントに表示されるフォルダの親フォルダです。 |
| 送信トレイ | 送信トレイ フォルダー。 |
| recoverableitemsdeletions | ソフト削除されたアイテムを含むフォルダ：[削除済みアイテム]フォルダから削除するか、OutlookでShift + Deleteキーを押して削除したアイテム。 このフォルダはどのOutlook電子メールクライアントにも表示されませんが、エンドユーザーはOutlookまたはWeb上のOutlookの**サーバーから削除済みアイテムを回復**機能を使用して操作できます。 |
| スケジュール済み | iOS用Outlookのスケジュール機能を使用して受信トレイに再表示されるようにスケジュールされているメッセージを含むフォルダ。 |
| searchfolders | ユーザーのメールボックスに定義されているすべての検索フォルダーの親フォルダー。 |
| sentitems | 送信済みアイテム フォルダー。 |
| serverfailures | サーバー上に存在するがローカルクライアントと同期できなかったアイテムを含むフォルダー。 |
| syncissues | Outlookによって作成された同期ログを含むフォルダー。 |

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
|[mailFolder の取得](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |mailFolder オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MailFolder の作成](../api/mailfolder-post-childfolders.md) |[MailFolder](mailfolder.md)| childFolders コレクションへの投稿により、現在の mailFolder 下に新しい mailFolder を作成します。|
|[childFolders を一覧表示する](../api/mailfolder-list-childfolders.md) |[MailFolder](mailfolder.md) コレクション| 指定したフォルダーの下のフォルダー コレクションを取得します。`.../me/MailFolders` ショートカットを使用すると、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。|
|[メッセージの作成](../api/mailfolder-post-messages.md) |[Message](message.md)| メッセージ コレクションへの投稿により、現在の mailFolder に新しいメッセージを作成します。|
|[List messages](../api/mailfolder-list-messages.md) |[Message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージや、メールボックス内の指定したフォルダー内のメッセージを取得します。|
|[更新する](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|指定した mailFolder オブジェクトを更新します。 |
|[削除](../api/mailfolder-delete.md) | なし |指定した mailFolder オブジェクトを削除します。 |
|[コピー](../api/mailfolder-copy.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder にコピーします。|
|[delta](../api/mailfolder-delta.md)|[mailFolder](mailfolder.md) コレクション|ユーザーのメールボックスで追加または削除された一連のメール フォルダーを取得します。|
|[move](../api/mailfolder-move.md)|[MailFolder](mailfolder.md)|mailFolder とその内容を別の mailFolder に移動します。|
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
|id|文字列|mailFolder の一意識別子。|
|parentFolderId|String|mailFolder の親 mailFolder の一意識別子。|
|totalItemCount|Int32|mailFolder に含まれるアイテムの数|
|unreadItemCount|Int32|mailFolder 内で未読としてマークされているアイテムの数。|

**アイテム数を効率的に取得する**

フォルダーの `TotalItemCount`プロパティと `UnreadItemCount` プロパティを使用すると、ファイル内の既読アイテム数を簡単に算出できます。
大幅な待ち時間を招く可能性がある次のようなクエリを避けることができます。

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlookのメールフォルダには複数の種類のアイテムを含めることができます。たとえば、受信トレイにはメールアイテムとは異なる会議出席依頼アイテムを含めることができます。 `TotalItemCount` と `UnreadItemCount` には、アイテムの種類に関係なく、フォルダー内のアイテム全てが含まれます。

## <a name="relationships"></a>関係

| リレーションシップ | 型 | 説明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) コレクション|mailFolder 内の子フォルダーのコレクション。|
|messageRules | [messageRule](messagerule.md) コレクション | ユーザーの受信トレイ フォルダーに適用されるルールのコレクション。 |
|messages|[Message](message.md) コレクション|mailFolder 内のメッセージのコレクション。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| mailFolder に対して定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| mailFolder に対して定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。|

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

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
