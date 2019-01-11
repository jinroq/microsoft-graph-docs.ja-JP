---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: a0f5d13381c82a42159d0802d850d9996aaf8b54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855182"
---
# <a name="numbercolumn-resource-type"></a>numberColumn リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ名      | Type   | 説明
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | 文字列 | 表示する小数点以下の桁数です。 使用可能な値については、下記を参照してください。
| **displayAs**      | 文字列 | UX での値の表示方法です。 `number` または `percentage` のいずれかでなければなりません。 指定しない場合、`number` として扱われます。
| **maximum**        | double | 許容最大値です。
| **minimum**        | double | 許容最小値です。

## <a name="decimalplaces-values"></a>DecimalPlaces values

| 値          | 説明
|:---------------|:--------------------------------------------------------------
| **automatic**  | 既定値。 必要に応じて自動的に小数点以下の桁を表示します。
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
  "tocPath": "Resources/NumberColumn"
} -->
