---
title: workbookTableRow リソースの種類
description: テーブル内の行を表します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e6097915005c96291f93543866ad9e28ff781f82
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963872"
---
# <a name="workbooktablerow-resource-type"></a>workbookTableRow リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テーブル内の行を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableRow を取得する　](../api/tablerow-get.md) | [workbookTableRow](workbooktablerow.md) |tableRow オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/tablerow-update.md) | [workbookTableRow](workbooktablerow.md)  |TableRow を更新します。 |
|[Range](../api/tablerow-range.md)|[workbookRange](workbookrange.md)|行全体に関連付けられた範囲オブジェクトを返します。|
|[Delete](../api/tablerow-delete.md)|None|テーブルから行を削除します。|
|[List](../api/tablerow-list.md) | [workbookTableRow](workbooktablerow.md)コレクション |tableRow オブジェクトのコレクションを取得します。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[workbookTableRow](workbooktablerow.md)|コレクション内の位置を基に行を取得します。|
|[Add](../api/tablerowcollection-add.md)|[workbookTableRow](workbooktablerow.md)|新しい行をテーブルに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|index|int|テーブルの行コレクション内の行のインデックス番号を返します。0 を起点とする番号になります。読み取り専用。|
|values|Json|指定した範囲の Raw 値を表します。返されるデータの型は、文字列、数値、またはブール値のいずれかになります。エラーが含まれているセルは、エラー文字列を返します。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookTableRow"
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
  "suppressions": []
}
-->
