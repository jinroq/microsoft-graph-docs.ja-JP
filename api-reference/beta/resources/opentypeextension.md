---
title: openTypeExtension リソース タイプ (オープン拡張機能)
description: (Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508833"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension リソース タイプ (オープン拡張機能)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

(Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。
オープン拡張機能は、**openTypeExtension** リソースで表されます。 リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。  各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。 拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。 拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。

オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)

オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。

| リソース | バージョン |
|---------------|-------|
| [管理単位](administrativeunit.md)  | プレビューのみ |
| [予定表イベント](event.md) | GA |
| グループ[予定表イベント](event.md) | GA |
| グループ会話スレッド[投稿](post.md) | GA |
| [device](device.md) | GA |
| [グループ](group.md) | GA |
| [メッセージ](message.md) | GA |
| [組織](organization.md) | GA |
| [個人用連絡先](contact.md) | GA |
| [ユーザー](user.md) | GA |

## <a name="outlook-specific-considerations"></a>Outlook に固有の考慮事項

(イベント、メッセージ、または個人用の連絡先)、Outlook のリソース上に存在の開いている各拡張機能は、 [MAPI の名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に格納されます。 Outlook を開いている拡張機能を作成するときは、MAPI プロパティを名前付きのユーザーのメールボックス内の有限のリソースであることを検討します。 ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対して複数の名前付きプロパティを作成できません。 その場合、関数の名前付きプロパティに依存するクライアントからの予期しない動作します。

Outlook のリソースで開いている拡張機能を作成するときは、次のガイドラインを適用します。

- 必要な拡張の最小数を作成します。 ほとんどのアプリケーションは、複数の拡張機能を必要があります。 拡張機能があるないプロパティの設定を定義または構造体は、単一の拡張機能に複数の値を格納することができますので。
- (などのユーザー入力などに基づきます)。 変数の方法で拡張機能の名前付けをしないでください。 前に、ユーザーのメールボックスで使用されていない新しい名前で開いている拡張機能を作成するたびに、新しい MAPI 名前付きプロパティが作成されます。 拡張子を削除しても、名前付きプロパティは削除されません。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>オープン拡張機能 (Outlook リソース用) と拡張プロパティのどちらを使用するか

保存して、カスタムのデータへのアクセスに関連するほとんどのシナリオで推奨されるソリューションを開いています。 ただし、 [Microsoft グラフ API メタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)を通じて公開されていない Outlook MAPI プロパティのカスタムのデータにアクセスする必要がある場合は、[拡張プロパティおよびその他の API](extended-properties-overview.md)を使用できます。 メタデータを公開するプロパティを確認することができます[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|extensionName|String|オープン型のデータ拡張情報の一意のテキスト識別子。必須。|
|id|String| **extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md)(既存リソースのインスタンスで)、または、[連絡先](../resources/contact.md)の新しい、[イベント](../resources/event.md)、または openTypeExtension オブジェクトを含む[メッセージ](../resources/message.md)です。 | 既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |openTypeExtension オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |openTypeExtension オブジェクトを更新します。 |
|[削除](../api/opentypeextension-delete.md) | なし |openTypeExtension オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
