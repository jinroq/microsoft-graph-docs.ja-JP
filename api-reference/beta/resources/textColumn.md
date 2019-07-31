---
author: JeremyKelley
description: columnDefinition リソースの textColumn は、列の値がテキストであることを示します。
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964342"
---
# <a name="textcolumn-resource-type"></a>TableColumn リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[columnDefinition](columndefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**textColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名                   | 種類   | 説明
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | string | この列への更新が既存のテキストを置き換えるか、または追加するか。
| **linesForEditing**             | int    | テキスト ボックスのサイズ。
| **maxLength**                   | int    | 値に使用できる最大文字数。
| **textType**                    | string | 格納されているテキストの種類。 `plain` または `richText` のいずれかでなければなりません。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
