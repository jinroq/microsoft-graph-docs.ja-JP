---
title: 傾向のあるリソースの種類
description: ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。 OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 90ebc84aa66fcd3dfd352d79256b725bf7a6d0e7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333576"
---
# <a name="trending-resource-type"></a>傾向のあるリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーに関連するドキュメントへのユーザー接続の高度な関係 (ユーザーに関連しています)。 OneDrive ファイル、および SharePoint チームサイトに保存されたファイルは、ユーザーの周囲での傾向があります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[人気上昇中を一覧表示する](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)コレクション| トレンドファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型                              | 説明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | リレーションシップの一意識別子。 読み取り専用です。        |
| weight                | 2 行分                    | ドキュメントの現在の傾向を示す値。 数値が大きいほど、ドキュメントは現在ユーザーの傾向を示しています (より関連性が高い)。 返されたドキュメントは、この値で並べ替えられます。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | ドキュメントの url や種類など、傾向ドキュメントの参照プロパティ。 |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | エンティティ        | トレンド分析ドキュメントに移動するために使用します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```
