---
title: openTypeExtension リソース タイプ (オープン拡張機能)
description: オープン拡張機能 (以前の Office 365 データ拡張機能) は、Microsoft Graph のリソースに型指定されていないプロパティを直接追加する簡単な方法を提供します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568906"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension リソース タイプ (オープン拡張機能)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オープン拡張機能 (以前の Office 365 データ拡張機能) は、Microsoft Graph のリソースに型指定されていないプロパティを直接追加する簡単な方法を提供します。
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

## <a name="outlook-specific-considerations"></a>Outlook 固有の考慮事項

Outlook リソース (イベント、メッセージ、または個人連絡先) に存在するオープン拡張機能は、 [MAPI の名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に格納されます。 Outlook 用のオープン拡張機能を作成するときは、MAPI という名前のプロパティがユーザーのメールボックス内の有限リソースであることを考慮してください。 ユーザーの名前付きプロパティのクォータを使い果たすと、そのユーザーに対して名前付きプロパティを作成することはできません。 これにより、名前付きプロパティに依存するクライアントから予期しない動作が発生する可能性があります。

Outlook リソースにオープン拡張機能を作成するときには、次のガイドラインを適用します。

- 必要な拡張機能の最小数を作成します。 ほとんどのアプリケーションでは、複数の内線番号は必要ありません。 拡張機能には設定されたプロパティや構造がなく、1つの内線番号に複数の値を格納できます。
- 名前付け拡張機能は、(ユーザー入力に基づいた場合など) 変数の方法で回避してください。 オープン拡張機能が、ユーザーのメールボックスで使用されていない新しい名前で作成されるたびに、新しい MAPI という名前のプロパティが作成されます。 拡張機能を削除しても、名前付きプロパティは削除されません。

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>オープン拡張機能 (Outlook リソースの場合) または拡張プロパティを使用する

オープン拡張機能は、カスタム データの格納およびカスタムデータへのアクセスを必要とするほとんどのシナリオに対して推奨されるソリューションです。 ただし、[拡張プロパティとこの REST API](https://developer.microsoft.com/graph/docs/overview/call_api) は、[Microsoft Graph API のメタデータ](extended-properties-overview.md)を通じてまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合に使用できます。 [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)でメタデータが公開するプロパティを確認できます。

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

## <a name="relationships"></a>関係

なし

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | [opentypeextension](opentypeextension.md)(既存のリソースインスタンスの場合)、または opentypeextension オブジェクトを含む新しい[連絡先](../resources/contact.md)、[イベント](../resources/event.md)、または[メッセージ](../resources/message.md)。 | 既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。|
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
