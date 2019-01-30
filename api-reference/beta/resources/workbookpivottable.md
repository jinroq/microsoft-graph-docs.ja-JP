---
title: ピボットテーブル リソースの種類
description: Excel のピボットテーブルを表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641107"
---
# <a name="pivottable-resource-type"></a>ピボットテーブル リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
