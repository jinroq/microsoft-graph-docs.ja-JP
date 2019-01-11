---
title: ChartPoint リソースの種類
description: グラフの系列のポイントを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: f9bf959407a93c6d58d088833e5e3e437ef41125
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876252"
---
# <a name="chartpoint-resource-type"></a>ChartPoint リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

グラフの系列のポイントを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get ChartPoint](../api/chartpoint-get.md) | [ChartPoint](chartpoint.md) |chartPoint オブジェクトのプロパティと関係を読み取ります。|
|[List](../api/chartpoint-list.md) | [ChartPoint](chartpoint.md) コレクション |chartPoint オブジェクトのコレクションを取得します。 |
|[Itemat](../api/chartpointscollection-itemat.md)|[ChartPoint](chartpoint.md)|データ系列内の位置に基づくポイントを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|value|object|グラフのポイントの値を返します。値の取得のみ可能です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[ChartPointFormat](chartpointformat.md)|グラフのポイントの書式設定プロパティをカプセル化します。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
