---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889209"
---
# <a name="pivottable-resource-type"></a>ピボットテーブル リソースの種類

Excel のピボットテーブルを表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookPivotTable を取得する](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/workbookpivottable-refresh.md)|なし|ピボットテーブルを更新します。 |
|[Refreshall](../api/workbookpivottable-refreshall.md)|なし|指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| ピボットテーブルの ID。 読み取り専用です。|
|name|String|ピボットテーブルの名前。    |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[WorkbookWorksheet](worksheet.md)| 現在のピボットテーブルを含んでいるワークシート。読み取り専用。   |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
