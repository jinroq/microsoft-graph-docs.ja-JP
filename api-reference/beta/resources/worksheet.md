---
title: ワークシート リソースの種類
description: Excel のワークシートは、セルのグリッドです。 データ、表、グラフなどを含めることができます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523477"
---
# <a name="worksheet-resource-type"></a>ワークシート リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel のワークシートは、セルのグリッドです。 データ、表、グラフなどを含めることができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ワークシートを取得する](../api/worksheet-get.md) | [Worksheet](worksheet.md) |ワークシート オブジェクトのプロパティと関係を読み取ります。|
|[グラフを作成する](../api/worksheet-post-charts.md) |[Chart](chart.md)| グラフ コレクションに投稿して、新しいグラフを作成します。|
|[名前を一覧表示する](../api/worksheet-list-names.md) |[NamedItem](nameditem.md) コレクション| ワークシートに関連付けられた名前付きアイテムのコレクションを取得します。|
|[グラフを一覧表示する](../api/worksheet-list-charts.md) |[Chart](chart.md) コレクション| グラフ オブジェクトのコレクションを取得します。|
|[テーブルを作成する](../api/worksheet-post-tables.md) |[Table](table.md)| テーブル コレクションに投稿して、新しいテーブルを作成します。|
|[テーブルを一覧表示する](../api/worksheet-list-tables.md) |[Table](table.md) コレクション| テーブル オブジェクトのコレクションを取得します。|
|[Update](../api/worksheet-update.md) | [Worksheet](worksheet.md)   |ワークシート オブジェクトを更新します。 |
|[Cell](../api/worksheet-cell.md)|[Range](range.md)|行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。|
|[Range](../api/worksheet-range.md)|[Range](range.md)|アドレスまたは名前で指定された範囲オブジェクトを取得します。|
|[Usedrange](../api/worksheet-usedrange.md)|[Range](range.md)|使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。|
|[削除](../api/worksheet-delete.md)|なし|ブックからワークシートを削除します。|
|[List](../api/worksheet-list.md) | [Worksheet](worksheet.md) コレクション |ワークシート オブジェクトのコレクションを取得します。 |
|[Add](../api/worksheetcollection-add.md)|[Worksheet](worksheet.md)|新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。 |
|[pivotTables を一覧表示する](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md) コレクション| workbookPivotTable オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|id|string|指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。|
|name|文字列|ワークシートの表示名。|
|position|int|0 を起点とした、ブック内のワークシートの位置。|
|visibility|string|ワークシートの可視性。可能な値は、`Visible`、`Hidden`、`VeryHidden` です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|charts|[Chart](chart.md) コレクション|ワークシートの一部になっているグラフのコレクションを返します。値の取得のみ可能です。|
|names|[NamedItem](nameditem.md) コレクション|ワークシートに関連付けられている名前のコレクションを返します。 値の取得のみ可能です。|
|テーブル|[workbookPivotTable](workbookpivottable.md) コレクション| ワークシートの一部になっているピボットテーブルのコレクション。 |
|protection|[WorksheetProtection](worksheetprotection.md)|ワークシートのシート保護オブジェクトを返します。読み取り専用です。|
|tables|[Table](table.md) コレクション|ワークシートの一部になっているグラフのコレクション。値の取得のみ可能です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
