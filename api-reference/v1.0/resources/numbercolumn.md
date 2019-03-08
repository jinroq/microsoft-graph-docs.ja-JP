---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: 42824275bd79f4b631d53365997d2dd96984f7b5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480853"
---
# <a name="numbercolumn-resource-type"></a>numberColumn リソースの種類

[columnDefinition](columndefinition.md) リソースの **numberColumn** は、列の値が数値であることを示します。

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

| プロパティ名      | 種類   | 説明
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | string | 表示する小数点以下の桁数です。 使用可能な値については、下記を参照してください。
| **displayAs**      | string | UX での値の表示方法です。 `number` または `percentage` のいずれかでなければなりません。 指定しない場合、`number` として扱われます。
| **maximum**        | double | 許容最大値です。
| **minimum**        | double | 許容最小値です。

## <a name="decimalplaces"></a>DecimalPlaces

| 値          | 説明
|:---------------|:--------------------------------------------------------------
| **automatic**  | 既定。 必要に応じて自動的に小数点以下の桁を表示します。
| **none**       | 小数点以下の桁は表示されません。
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
