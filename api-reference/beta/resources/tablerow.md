---
title: TableRow リソースの種類
description: 表の行を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e1c9dc0f9aad61d815098b76da8620d808c2538a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643749"
---
# <a name="tablerow-resource-type"></a>TableRow リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表の行を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableRow を取得する](../api/tablerow-get.md) | [TableRow](tablerow.md) |tableRow オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/tablerow-update.md) | [TableRow](tablerow.md)  |TableRow を更新します。 |
|[Range](../api/tablerow-range.md)|[Range](range.md)|行全体に関連付けられた範囲オブジェクトを返します。|
|[削除する](../api/tablerow-delete.md)|なし|テーブルから行を削除します。|
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablerow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
