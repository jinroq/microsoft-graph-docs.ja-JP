---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
ms.openlocfilehash: 5433b5b5a76d313f8f34e460400906479e6d3d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876056"
---
# <a name="calculatedcolumn-resource-type"></a>CalculatedColumn リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ名  | Type    | 説明
|:---------------|:--------|:--------------------------------------------------
| **format**     | 文字列  | `dateTime` 出力の種類に対する値の形式。 `dateOnly` または `dateTime` のいずれかでなければなりません。
| **formula**    | 文字列  | この列の値を計算するために使用する数式。
| **outputType** | 文字列  | この列の値の形式を設定するために使用する出力の種類。 `boolean`、`currency`、`dateTime`、`number`、`text` のいずれかでなければなりません。

SharePoint の数式は、Excel の数式のような構文を使用します。
詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
