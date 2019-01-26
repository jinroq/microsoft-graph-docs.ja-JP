---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 587b52107f3a7f9892603afb8273ce55b6faa549
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577411"
---
# <a name="trending-resource-type"></a>トレンド ・ リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[リストのトレンド分析](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)コレクション| トレンド ・ ファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型                              | 説明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | リレーションシップの一意の識別子です。 読み取り専用です。        |
| weight                | 倍精度浮動小数点数                    | どれだけドキュメントが現在のトレンド分析を示す値です。 大きい番号より文書が現在のトレンド分析ユーザー (関連するほどである)。 返されたドキュメントは、この値で並べ替えられます。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)コレクション | プロパティは、時にドキュメントをビジュアル化を使用することができます。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)コレクション | トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。 |

## <a name="relationships"></a>関係

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | エンティティのコレクション | トレンドのドキュメントに移動するために使用されます。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trending"
}-->
```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
