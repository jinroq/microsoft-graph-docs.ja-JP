---
title: テーブル リソースの種類
description: Excel の表を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2e3e9c93f7459d666fbe7f28a67241c2831b7079
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642647"
---
# <a name="table-resource-type"></a>テーブル リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel の表を表します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[テーブルを取得する](../api/table-get.md) | [Table](table.md) |テーブル オブジェクトのプロパティと関係を読み取ります。|
|[TableColumn を作成する](../api/table-post-columns.md) |[TableColumn](tablecolumn.md)| 列コレクションに投稿して、新しい TableColumn を作成します。|
|[列を一覧表示する](../api/table-list-columns.md) |[TableColumn](tablecolumn.md) コレクション| TableColumn オブジェクトのコレクションを取得します。|
|[TableRow を作成します。](../api/table-post-rows.md) |[TableRow](tablerow.md)| 行コレクションに投稿して、新しい TableRow を作成します。|
|[行を一覧表示する](../api/table-list-rows.md) |[TableRow](tablerow.md) コレクション| TableRow オブジェクトのコレクションを取得します。|
|[Update](../api/table-update.md) | [Table](table.md)   |テーブル オブジェクトを更新します。 |
|[Databodyrange](../api/table-databodyrange.md)|[Range](range.md)|テーブルのデータ本体に関連付けられた範囲オブジェクトを取得します。|
|[Headerrowrange](../api/table-headerrowrange.md)|[Range](range.md)|テーブルのヘッダー行に関連付けられた範囲オブジェクトを取得します。|
|[Range](../api/table-range.md)|[Range](range.md)|テーブル全体に関連付けられた範囲オブジェクトを取得します。|
|[Totalrowrange](../api/table-totalrowrange.md)|[Range](range.md)|テーブルの集計行に関連付けられた範囲オブジェクトを取得します。|
|[Clearfilters](../api/table-clearfilters.md)|なし|現在テーブルに適用されているすべてのフィルターをクリアします。|
|[Converttorange](../api/table-converttorange.md)|[Range](range.md)|テーブルを通常の範囲のセルに変換します。すべてのデータが保持されます。|
|[Delete](../api/table-delete.md)|なし|テーブルを削除します。|
|[Reapplyfilters](../api/table-reapplyfilters.md)|なし|現在テーブルにあるすべてのフィルターを再適用します。|
|[List](../api/table-list.md) | [Table](table.md) コレクション |テーブル オブジェクトのコレクションを取得します。 |
|[Add](../api/tablecollection-add.md)|[Table](table.md)|新しいテーブルを作成します。範囲のソース アドレスにより、テーブルが追加されるワークシートが判断されます。テーブルが追加できない場合 (たとえば、アドレスが無効な場合や、テーブルが別のテーブルと重複している場合) は、エラーがスローされます。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|指定されたブックのテーブルを一意に識別する値を返します。 識別子の値は、テーブルの名前が変更された場合も変わりません。 このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。 読み取り専用。|
|name|string|テーブルの名前。|
|showHeaders|boolean|ヘッダー行を表示するかどうかを示します。この値によって、ヘッダー行の表示または削除を設定できます。|
|showTotals|boolean|集計行を表示するかどうかを示します。この値によって、集計行の表示または削除を設定できます。|
|style|string|テーブル スタイルを表す定数値。使用可能な値は次のとおりです。TableStyleLight1 から TableStyleLight21、TableStyleMedium1 から TableStyleMedium28、TableStyleStyleDark1 から TableStyleStyleDark11。ブックに存在するカスタムのユーザー定義スタイルも指定できます。|
|highlightFirstColumn|Boolean|最初の列に特別な書式設定が含まれているかどうかを示します。   |
|highlightLastColumn|Boolean|最後の列に特別な書式設定が含まれているかどうかを示します。 |
|showBandedColumns|Boolean|テーブルを見やすくするため、奇数列を偶数列とは異なる方法で強調表示する書式設定にして、列を縞模様で表示するかどうかを示します。   |
|showBandedRows|Boolean|テーブルを見やすくするため、奇数行を偶数行とは異なる方法で強調表示する書式設定にして、行を縞模様で表示するかどうかを示します。    |
|showFilterButton|Boolean|フィルター ボタンを各列のヘッダーの上部に表示するかどうかを示します。これは、テーブルにヘッダー行が含まれている場合のみ設定できます。   |
|legacyId|String|以前の Excle クライアントで使用されていたレガシ Id です。 識別子の値は、テーブルの名前が変更された場合も変わりません。 このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。 読み取り専用。   |

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|columns|[TableColumn](tablecolumn.md) コレクション|テーブルに含まれるすべての列のコレクションを表します。読み取り専用です。|
|rows|[TableRow](tablerow.md) コレクション|テーブルに含まれるすべての行のコレクションを表します。読み取り専用です。|
|sort|[TableSort](tablesort.md)|テーブル内の並べ替えを表します。読み取り専用。|
|worksheet|[Worksheet](worksheet.md)|現在のテーブルを含んでいるワークシート。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "@odata.type": "microsoft.graph.table"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/table.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
