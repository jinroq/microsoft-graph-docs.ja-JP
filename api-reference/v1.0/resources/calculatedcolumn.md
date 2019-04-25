---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 66fbc59fa9fe4880c023086c9bd334e04650bc73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569369"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn リソースの種類

[columnDefinition](columndefinition.md) リソースの **calculatedColumn** は、列のデータがサイト内の他の列に基づいて計算されることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**calculatedColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>プロパティ

| プロパティ名  | 種類    | 説明
|:---------------|:--------|:--------------------------------------------------
| **format**     | string  | `dateTime` 出力の種類に対する値の形式。 `dateOnly` または `dateTime` のいずれかでなければなりません。
| **formula**    | string  | この列の値を計算するために使用する数式。
| **outputType** | string  | この列の値の形式を設定するために使用する出力の種類。 `boolean`、`currency`、`dateTime`、`number`、`text` のいずれかでなければなりません。

SharePoint の数式は、Excel の数式のような構文を使用します。
詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->
