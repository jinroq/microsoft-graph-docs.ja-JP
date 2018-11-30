---
title: エンドポイント リソースの種類
description: 'エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 '
ms.openlocfilehash: 8d95cef8e25095512e94d5aed5ec7540562862bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068110"
---
# <a name="endpoint-resource-type"></a>エンドポイント リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[エンドポイントのリスト](../api/group-list-endpoints.md) |[エンドポイント](endpoint.md)のコレクション| エンドポイント オブジェクトのコレクションを取得します。 |
|[エンドポイントを取得します。](../api/endpoint-get.md) | [エンドポイント](endpoint.md) |エンドポイント オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| capability     | String  | このリソースに関連付けられている機能をについて説明します。 (例: メッセージ、会話など) Null を許容しません。 読み取り専用。 |
| id             | String  | エンドポイントの一意の識別子キーです。 null 許容ではありません。 読み取り専用です。|
| providerId     | String  | アプリケーション id が公開するサービスの基になるのです。 null 許容ではありません。 読み取り専用です。|
| プロバイダー   | String  | 公開するサービスの基になるの名前です。 読み取り専用。|
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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->