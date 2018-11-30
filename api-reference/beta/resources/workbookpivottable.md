---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
ms.openlocfilehash: 3cba1263715400def6b66149ecec11eddde5e686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072407"
---
# <a name="pivottable-resource-type"></a>ピボットテーブル リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Excel のピボットテーブルを表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookPivotTable を取得する](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/workbookpivottable-refresh.md)|なし|ピボットテーブルを更新します。 |
|[Refreshall](../api/workbookpivottable-refreshall.md)|なし|指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| ピボットテーブルの ID。 読み取り専用です。|
|name|String|ピボットテーブルの名前。    |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[worksheet](worksheet.md)| 現在のピボットテーブルを含んでいるワークシート。読み取り専用です。   |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
