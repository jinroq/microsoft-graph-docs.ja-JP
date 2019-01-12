---
title: TableRow リソースの種類
description: 表の行を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d96ef5c23361cd8b15b47af54a0584e21c48b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971663"
---
# <a name="tablerow-resource-type"></a>TableRow リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

表の行を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableRow を取得する](../api/tablerow-get.md) | [TableRow](tablerow.md) |tableRow オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/tablerow-update.md) | [TableRow](tablerow.md)  |TableRow を更新します。 |
|[Range](../api/tablerow-range.md)|[Range](range.md)|行全体に関連付けられた範囲オブジェクトを返します。|
|[Delete](../api/tablerow-delete.md)|なし|テーブルから行を削除します。|
|[List](../api/tablerow-list.md) | [TableRow](tablerow.md) コレクション |tableRow オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|コレクション内の位置を基に行を取得します。|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|新しい行をテーブルに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|index|int|テーブルの行コレクション内の行のインデックス番号を返します。0 を起点とする番号になります。読み取り専用。|
|values|json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
