---
title: 範囲リソースの種類
description: 範囲は、1 つ以上の隣接するセル (セル、行、列、セルのブロックなど) のセットを表します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 537da7c6a7b54c7977056ca822c4b98c85f2c1a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918949"
---
# <a name="range-resource-type"></a>範囲リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

範囲は、1 つ以上の隣接するセル (セル、行、列、セルのブロックなど) のセットを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[範囲を取得する](../api/range-get.md) | [Range](range.md) |範囲オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/range-update.md) | [Range](range.md)   |範囲オブジェクトを更新します。 |
|[Boundingrect](../api/range-boundingrect.md)|[Range](range.md)|指定した範囲を包含する、最小の範囲オブジェクトを取得します。たとえば、"B2:C5" と "D10:E15" の GetBoundingRect は、"B2:E16" になります。|
|[Cell](../api/range-cell.md)|[Range](range.md)|行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。|
|[列](../api/range-column.md)|[Range](range.md)|範囲に含まれる列を 1 つ取得します。|
|[Columnsafter](../api/workbookrange-columnsafter.md)|[workbookRangeView](workbookrangeview.md)|指定した範囲の右にある特定の列数を取得します。|
|[Columnsbefore](../api/workbookrange-columnsbefore.md)|[workbookRangeView](workbookrangeview.md)|指定した範囲の左にある特定の列数を取得します。|
|[Entirecolumn](../api/range-entirecolumn.md)|[Range](range.md)|範囲に含まれるすべての列を表すオブジェクトを取得します。|
|[Entirerow](../api/range-entirerow.md)|[Range](range.md)|範囲に含まれるすべての行を表すオブジェクトを取得します。|
|[Intersection](../api/range-intersection.md)|[Range](range.md)|指定した範囲の長方形の交差部分を表す範囲オブジェクトを取得します。|
|[Lastcell](../api/range-lastcell.md)|[Range](range.md)|範囲内の最後のセルを取得します。たとえば、"B2:D5" の最後のセルは "D5" になります。|
|[Lastcolumn](../api/range-lastcolumn.md)|[Range](range.md)|範囲内の最後の列を取得します。たとえば、"B2:D5" の最後の列は "D2:D5" になります。|
|[Lastrow](../api/range-lastrow.md)|[Range](range.md)|範囲内の最後の行を取得します。たとえば、"B2:D5" の最後の行は "B5:D5" になります。|
|[Offsetrange](../api/range-offsetrange.md)|[Range](range.md)|指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。|
|[行](../api/range-row.md)|[Range](range.md)|範囲に含まれている行を 1 つ取得します。|
|[Rowsabove](../api/workbookrange-rowsabove.md)|[workbookRangeView](workbookrangeview.md)|指定した範囲の上にある特定の行数を取得します。|
|[Rowsbelow](../api/workbookrange-rowsbelow.md)|[workbookRangeView](workbookrangeview.md)|指定した範囲の下にある特定の行数を取得します。|
|[Usedrange](../api/range-usedrange.md)|[Range](range.md)|指定した範囲オブジェクトのうち使用されている範囲を返します。|
|[Clear](../api/range-clear.md)|なし|範囲の値、書式、塗りつぶし、罫線などをクリアします。|
|[Delete](../api/range-delete.md)|なし|範囲に関連付けられているセルを削除します。|
|[Insert](../api/range-insert.md)|[Range](range.md)|この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。|
|[Merge](../api/range-merge.md)|なし|範囲内のセルをワークシートの 1 つの領域に結合します。|
|[Resizedrange](../api/workbookrange-resizedrange.md)|[workbookRangeView](workbookrangeview.md)|現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。|
|[Unmerge](../api/range-unmerge.md)|なし|範囲内のセルを結合解除して別々のセルにします。|
|[Visibleview](../api/workbookrange-visibleview.md)|[workbookRangeView](workbookrangeview.md)|フィルター済み範囲から、表示されている範囲を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|address|文字列|A1 スタイルの範囲参照を表します。アドレス値には、シート参照が格納されます (例: Sheet1!A1:B4)。読み取り専用です。|
|addressLocal|文字列|ユーザーの言語で指定された範囲の範囲参照を表します。読み取り専用です。|
|cellCount|int|範囲に含まれるセルの数。読み取り専用です。|
|columnCount|int|範囲に含まれる列の合計数を表します。読み取り専用です。|
|columnHidden|ブール値|現在の範囲のすべての列が非表示になっているかどうかを表します。|
|columnIndex|int|範囲に含まれる最初のセルの列番号を表します。0 を起点とする番号になります。読み取り専用です。|
|formulas|json|A1 スタイル表記の数式を表します。|
|formulasLocal|json|ユーザーの言語と数値書式ロケールで、A1 スタイル表記の数式を表します。たとえば、英語の数式 "=SUM(A1, 1.5)" は、ドイツ語では "=SUMME(A1; 1,5)" になります。|
|formulasR1C1|json|R1C1 スタイル表記の数式を表します。|
|hidden|ブール値|現在の範囲のすべてのセルが非表示になっているかどうかを表します。読み取り専用です。|
|numberFormat|json|指定したセルの Excel の数値書式コードを表します。|
|rowCount|int|範囲に含まれる行の合計数を返します。読み取り専用です。|
|rowHidden|ブール値|現在の範囲のすべての行が非表示になっているかどうかを表します。|
|rowIndex|int|範囲に含まれる最初のセルの行番号を返します。0 を起点とする番号になります。読み取り専用です。|
|text|json|指定した範囲のテキスト値。テキスト値は、セルの幅には依存しません。Excel UI で発生する # 記号による置換は、この API から返されるテキスト値には影響しません。読み取り専用です。|
|valueTypes|文字列|各セルのデータの種類を表します。可能な値は、`Unknown`、`Empty`、`String`、`Integer`、`Double`、`Boolean`、`Error` です。読み取り専用です。|
|values|json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|format|[RangeFormat](rangeformat.md)|Format オブジェクト (範囲のフォント、塗りつぶし、罫線、配置などのプロパティをカプセル化するオブジェクト) を返します。読み取り専用です。|
|sort|[RangeSort](rangesort.md)|現在の範囲を含んでいるワークシート。読み取り専用です。|
|worksheet|[Worksheet](worksheet.md)|現在の範囲を含んでいるワークシート。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.range"
}-->

```json
{
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "json",
  "formulasLocal": "json",
  "formulasR1C1": "json",
  "hidden": true,
  "numberFormat": "json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
