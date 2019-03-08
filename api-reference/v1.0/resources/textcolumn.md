---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480839"
---
# <a name="textcolumn-resource-type"></a>TableColumn リソースの種類

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

| プロパティ名                   | 種類    | 説明
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | ブール値 | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | ブール値 | この列への更新が既存のテキストを置き換えるか、または追加するか。
| **linesForEditing**             | int32   | テキスト ボックスのサイズ。
| **maxLength**                   | int32   | 値に使用できる最大文字数。
| **textType**                    | string  | 格納されているテキストの種類。 `plain` または `richText` のいずれかでなければなりません。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
