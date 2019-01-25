---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507496"
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
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | プロパティは、時にドキュメントをビジュアル化を使用することができます。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。 |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | Entity        | トレンドのドキュメントに移動するために使用されます。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

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
