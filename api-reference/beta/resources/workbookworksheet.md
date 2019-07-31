---
title: workbookWorksheet リソースの種類
description: Excel のワークシートは、セルのグリッドです。 データ、表、グラフなどを含めることができます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 93386edf60e30069068ceb2fa437fb128b239302
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963858"
---
# <a name="workbookworksheet-resource-type"></a>workbookWorksheet リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel のワークシートは、セルのグリッドです。 データ、表、グラフなどを含めることができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ワークシートを取得する](../api/worksheet-get.md) | [workbookWorksheet](workbookworksheet.md) |ワークシート オブジェクトのプロパティと関係を読み取ります。|
|[グラフを作成する](../api/worksheet-post-charts.md) |[workbookChart](workbookchart.md)| グラフ コレクションに投稿して、新しいグラフを作成します。|
|[名前を一覧表示する](../api/worksheet-list-names.md) |[workbookNamedItem](workbooknameditem.md)コレクション| ワークシートに関連付けられている名前付きのアイテムのコレクションを取得します。|
|[グラフを一覧表示する](../api/worksheet-list-charts.md) |[workbookChart](workbookchart.md)コレクション| グラフ オブジェクトのコレクションを取得します。|
|[テーブルを作成する](../api/worksheet-post-tables.md) |[workbookTable](workbooktable.md)| テーブル コレクションに投稿して、新しいテーブルを作成します。|
|[テーブルを一覧表示する](../api/worksheet-list-tables.md) |[workbookTable](workbooktable.md)コレクション| テーブル オブジェクトのコレクションを取得します。|
|[Update](../api/worksheet-update.md) | [workbookWorksheet](workbookworksheet.md)   |ワークシート オブジェクトを更新します。 |
|[Cell](../api/worksheet-cell.md)|[workbookRange](workbookrange.md)|行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。|
|[Range](../api/worksheet-range.md)|[workbookRange](workbookrange.md)|アドレスまたは名前で指定された範囲オブジェクトを取得します。|
|[Usedrange](../api/worksheet-usedrange.md)|[workbookRange](workbookrange.md)|使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。|
|[Delete](../api/worksheet-delete.md)|なし|ブックからワークシートを削除します。|
|[List](../api/worksheet-list.md) | [workbookWorksheet](workbookworksheet.md)コレクション |ワークシート オブジェクトのコレクションを取得します。 |
|[Add](../api/worksheetcollection-add.md)|[workbookWorksheet](workbookworksheet.md)|新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。 |
|[pivotTables を一覧表示する](../api/workbookworksheet-list-pivottables.md) |[workbookPivotTable](workbookpivottable.md) コレクション| workbookPivotTable オブジェクト コレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|指定されたブックのワークシートを一意に識別する値を返します。この識別子の値は、ワークシートの名前を変更したり移動したりしても同じままです。値の取得のみ可能です。|
|name|string|ワークシートの表示名。|
|position|int|0 を起点とした、ブック内のワークシートの位置。|
|visibility|string|ワークシートの可視性。 使用可能な値: `Visible`、`Hidden`、`VeryHidden`。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|グラフ|[workbookChart](workbookchart.md)コレクション|ワークシートの一部になっているグラフのコレクションを返します。 読み取り専用です。|
|names|[workbookNamedItem](workbooknameditem.md)コレクション|ワークシートに関連付けられている名前のコレクションを返します。 値の取得のみ可能です。|
|pivotTables|[workbookPivotTable](workbookpivottable.md) コレクション| ワークシートの一部になっているピボットテーブルのコレクション。 |
|保護|[workbookWorksheetProtection](workbookworksheetprotection.md)|ワークシートのシート保護オブジェクトを返します。読み取り専用です。|
|テーブル|[workbookTable](workbooktable.md)コレクション|ワークシートの一部になっているグラフのコレクション。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
  "suppressions": []
}
-->
