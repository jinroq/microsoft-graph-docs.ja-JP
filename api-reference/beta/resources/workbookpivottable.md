---
title: workbookPivotTable リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d8df88699fde1e4d5562db6299cd12665512c03b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963994"
---
# <a name="workbookpivottable-resource-type"></a>workbookPivotTable リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel のピボットテーブルを表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[workbookPivotTable を取得する](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |worksheetprotection オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新](../api/workbookpivottable-refresh.md)|None|ピボットテーブルを更新します。 |
|[Refreshall](../api/workbookpivottable-refreshall.md)|なし|指定したワークシート内のすべてのテーブルを更新します。このアクションは、ピボットテーブルのコレクションでのみ使用できることに注意してください。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|文字列| ピボットテーブルの ID。 読み取り専用です。|
|name|String|ピボットテーブルの名前。    |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[workbookWorksheet](workbookworksheet.md)| 現在のピボットテーブルを含んでいるワークシート。 読み取り専用です。   |

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
