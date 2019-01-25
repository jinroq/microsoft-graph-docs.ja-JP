---
title: エンドポイント リソースの種類
description: 'エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512060"
---
# <a name="endpoint-resource-type"></a>エンドポイント リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[エンドポイントを一覧表示する](../api/group-list-endpoints.md) |[Endpoint](endpoint.md) collection| endpoint オブジェクトのコレクションを取得します。 |
|[エンドポイントを取得する](../api/endpoint-get.md) | [エンドポイント](endpoint.md) |endpoint オブジェクトのプロパティと関係を読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| capability     | String  | このリソースに関連付けられている機能をについて説明します。 (例: メッセージ、会話など) Null を許容しません。 読み取り専用です。 |
| id             | String  | エンドポイントの一意の識別子キーです。 null 許容ではありません。 読み取り専用です。|
| ProviderID     | String  | アプリケーション id が公開するサービスの基になるのです。 null 許容ではありません。 読み取り専用です。|
| ProviderName   | String  | 公開するサービスの基になるの名前です。 読み取り専用です。|
| providerResourceId|String| Office 365 グループでは、この処理は、リソース (たとえば Yammer.FeedURL など) の既知の名前に設定されます。 null 許容ではありません。 読み取り専用です。|
| uri            | String  | 公開されたリソースの URL です。 null 許容ではありません。 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ

なし。


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
