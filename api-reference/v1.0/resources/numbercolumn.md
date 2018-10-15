---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266507"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn リソース型

[columnDefinition](columnDefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**numberColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>プロパティ

| プロパティ名      | 型   | 説明
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | string | 表示する小数点以下の桁数です。 使用可能な値については、下記を参照してください。
| **displayAs**      | string | UX での値の表示方法です。 または `percentage` のいずれかでなければなりません。`number` 指定しない場合、`number` として扱われます。
| **maximum**        | double | 許容最大値です。
| **minimum**        | double | 許容最小値です。

## <a name="decimalplaces"></a>decimalPlaces

| 値          | 説明
|:---------------|:--------------------------------------------------------------
| **automatic**  | 既定。 必要に応じて自動的に小数点以下の桁を表示します。
| **なし**       | 小数点以下の桁は表示されません。
| **one**        | 小数第 1 位までを常に表示します。
| **two**        | 小数第 2 位までを常に表示します。
| **three**      | 小数第 3 位までを常に表示します。
| **four**       | 小数第 4 位までを常に表示します。
| **five**       | 小数第 5 位までを常に表示します。

注: **decimalPlaces** と **displayAs** は数値の格納方法ではなく、表示方法に適用されます。
これらのプロパティは更新される場合があります。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
