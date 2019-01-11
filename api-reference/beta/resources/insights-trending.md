---
title: トレンド ・ リソースの種類
description: ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: dc0154d3985e5f6e1e4770bb7d10bc727a0eb0ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862385"
---
# <a name="trending-resource-type"></a>トレンド ・ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザー (は、ユーザーに関連する) 傾向を示しているドキュメントへのユーザーの接続の豊富な関係です。 OneDrive ファイルでは、チームの SharePoint サイトにファイルを保存できるユーザー傾向があるとします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[リストのトレンド分析](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)コレクション| トレンド ・ ファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ      | 種類                              | 説明  |
| ------------- |---------------                    | -------------|
| ID                    | String                    | リレーションシップの一意の識別子です。 読み取り専用です。        |
| weight                | 倍精度浮動小数点数                    | どれだけドキュメントが現在のトレンド分析を示す値です。 大きい番号より文書が現在のトレンド分析ユーザー (関連するほどである)。 返されたドキュメントは、この値で並べ替えられます。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | プロパティは、時にドキュメントをビジュアル化を使用することができます。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | トレンド ・ ドキュメント、url、ドキュメントの種類などのプロパティを参照します。 |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 種類          | 説明  |
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
