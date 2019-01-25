---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: cf1f6c6cafd23a5503d645d13e597a8941019fee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512879"
---
# <a name="numbercolumn-resource-type"></a>numberColumn リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="decimalplaces-values"></a>DecimalPlaces values

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
