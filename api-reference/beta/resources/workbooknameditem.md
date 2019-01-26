---
title: WorkbookNamedItem リソースの種類
description: セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。
localization_priority: Normal
ms.openlocfilehash: 79ed5211c60555d2cfc55e01c49565ebecd58a8b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579850"
---
# <a name="nameditem-resource-type"></a>NamedItem リソースの種類

セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[workbookNameditem](workbooknameditem.md)|新しい名前を指定したスコープのコレクションに追加します。|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[workbookNameditem](workbooknameditem.md)|ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。|
|[NamedItem を取得する](../api/nameditem-get.md) | [workbookNameditem](workbooknameditem.md) |namedItem オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/nameditem-update.md) | [workbookNameditem](workbooknameditem.md)   |NamedItem オブジェクトを更新します。 |
|[Range](../api/nameditem-range.md)|[range](range.md)|名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。|
|[List](../api/nameditem-list.md) | [workbookNameditem](workbooknameditem.md)コレクション |namedItem オブジェクトのコレクションを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|文字列|オブジェクトの名前。読み取り専用です。|
|comment|文字列|この名前に関連付けられているコメントを表します。|
|scope|文字列|名前がブックを対象にしているのか、特定のワークシートを対象にしているのかを示します。読み取り専用です。|
|type|文字列|名前に関連付けられている参照の型を示します。可能な値は、`String`、`Integer`、`Double`、`Boolean`、`Range` です。読み取り専用です。|
|value|文字列|定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。|
|visible|boolean|オブジェクトを表示するかどうかを指定します。|

## <a name="relationships"></a>関係
| リレーションシップ     | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[workbookWorksheet](worksheet.md)|名前付きのアイテムの対象になるワークシートを返します。アイテムの対象がワークシートの場合にのみ使用できます。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
