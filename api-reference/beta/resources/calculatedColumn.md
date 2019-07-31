---
author: JeremyKelley
description: columnDefinition リソースの calculatedColumn は、列のデータがサイト内の他の列に基づいて計算されることを示します。
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8492dcf39cbdee92a998a418599fc00b314078c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013060"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->
