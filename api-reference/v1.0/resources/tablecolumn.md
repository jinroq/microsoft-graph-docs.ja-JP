---
title: TableColumn リソースの種類
description: テーブル内にある 1 つの列を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 095317b36c5242cd5e78f58192a242bd4e1f2993
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033979"
---
# <a name="tablecolumn-resource-type"></a>TableColumn リソースの種類

テーブル内にある 1 つの列を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableColumn を取得する](../api/tablecolumn-get.md) | [WorkbookTableColumn](tablecolumn.md) |tableColumn オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/tablecolumn-update.md) | [WorkbookTableColumn](tablecolumn.md) |TableColumn オブジェクトを更新します。 |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[Range](range.md)|列のデータ本体に関連付けられた範囲オブジェクトを取得します。|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[Range](range.md)|列のヘッダー行に関連付けられた範囲オブジェクトを取得します。|
|[Range](../api/tablecolumn-range.md)|[Range](range.md)|列全体に関連付けられた範囲オブジェクトを取得します。|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[Range](range.md)|列の集計行に関連付けられた範囲オブジェクトを取得します。|
|[Delete](../api/tablecolumn-delete.md)|None|テーブルから列を削除します。|
|[List](../api/tablecolumn-list.md) | [WorkbookTableColumn](tablecolumn.md) コレクション |tableColumn オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablecolumncollection-itemat.md)|[WorkbookTableColumn](tablecolumn.md)|コレクション内の位置に基づいて列を取得します。|
|[Add](../api/tablecolumncollection-add.md)|[WorkbookTableColumn](tablecolumn.md)|テーブルに新しい列を追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|テーブル内の列を識別する一意のキーを返します。 このプロパティは符号化文字列値として解釈し、その他の型に解析すべきではありません。 読み取り専用。|
|index|int|テーブルの列コレクション内の列のインデックス番号を返します。0 を起点とする番号になります。読み取り専用です。|
|name|string|テーブル列の名前を取得します。読み取り専用です。|
|values|Json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|フィルター|[WorkbookFilter](filter.md)|列に適用されるフィルターを取得します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
