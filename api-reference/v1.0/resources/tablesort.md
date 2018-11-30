---
title: TableSort リソースの種類
description: テーブル オブジェクトの並べ替え操作を管理します。
ms.openlocfilehash: 3696608f13e4a56b71a84bc2d287300e9e54cfb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024290"
---
# <a name="tablesort-resource-type"></a>TableSort リソースの種類

テーブル オブジェクトの並べ替え操作を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableSort を取得する](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |tableSort オブジェクトのプロパティと関係を読み取ります。|
|[適用](../api/tablesort-apply.md)|なし|並べ替え操作を実行します。|
|[クリア](../api/tablesort-clear.md)|なし|テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。|
|[Reapply](../api/tablesort-reapply.md)|なし|テーブルに、現在の並べ替えパラメーターを再適用します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md)コレクション|テーブルの最後の並べ替えに使用する現在の条件を表します。読み取り専用です。|
|matchCase|ブール値|大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。|
|method|文字列|中国語の文字が最後にテーブルの並べ替えに使用するメソッドの順序を表します。 可能な値: `PinYin`、 `StrokeCount`。 読み取り専用。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->