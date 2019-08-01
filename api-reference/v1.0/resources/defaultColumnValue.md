---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: columnDefinition リソースの defaultColumnValue は、この列の既定値を指定します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029513"
---
# <a name="defaultcolumnvalue-resource-type"></a>DefaultColumnValue リソースの種類

[columnDefinition](columndefinition.md) リソースの **defaultColumnValue** は、この列の既定値を指定します。
既定値は直接または数式として指定できます。

## <a name="json-representation"></a>JSON 表記

以下は、**defaultColumnValue** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| **formula**   | string | この列の既定値を計算するために使用する数式。
| **value**     | string | この列の既定値として使用する直接値。

一度に**数式**または**値**のうちの 1 つだけを指定することができます。

SharePoint の数式は、Excel の数式のような構文を使用します。
詳細については、「[SharePoint リストの一般的な数式の例][SPFormulas]」を参照してください。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
