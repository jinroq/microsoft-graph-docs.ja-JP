---
title: NamedItem リソースの種類
description: セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。
localization_priority: Normal
ms.openlocfilehash: e413361cc42a0f8f65e23e12d36b49d2c7bcebb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548526"
---
# <a name="nameditem-resource-type"></a>NamedItem リソースの種類

セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[WorkbookNamedItem](nameditem.md)|新しい名前を指定したスコープのコレクションに追加します。|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。|
|[NamedItem を取得する](../api/nameditem-get.md) | [WorkbookNamedItem](nameditem.md) |namedItem オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/nameditem-update.md) | [WorkbookNamedItem](nameditem.md)   |NamedItem オブジェクトを更新します。 |
|[Range](../api/nameditem-range.md)|[Range](range.md)|名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。|
|[List](../api/nameditem-list.md) | [WorkbookNamedItem](nameditem.md) コレクション |namedItem オブジェクトのコレクションを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|string|オブジェクトの名前。読み取り専用です。|
|comment|string|この名前に関連付けられているコメントを表します。|
|scope|string|名前がブックを対象にしているのか、特定のワークシートを対象にしているのかを示します。読み取り専用です。|
|type|string|名前に関連付けられている参照の型を示します。 使用可能な値: `String`、`Integer`、`Double`、`Boolean`、`Range`。 読み取り専用です。|
|value|Json|定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。|
|visible|ブール値|オブジェクトを表示するかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ     | 型   |説明|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)|名前付きのアイテムの対象になるワークシートを返します。アイテムの対象がワークシートの場合にのみ使用できます。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
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
