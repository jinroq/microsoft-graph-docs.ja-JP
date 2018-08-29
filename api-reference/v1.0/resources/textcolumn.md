---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: b5c41091b9193aabc36ee04e9dcc310bfc110af1
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264288"
---
# <a name="textcolumn-resource-type"></a>TableColumn リソースの種類

[columnDefinition](columnDefinition.md) リソースの **textColumn** は、列の値がテキストであることを示します。

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

| プロパティ名                   | 型    | 説明
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | ブール値 | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | ブール値 | この列への更新が既存のテキストを置き換えるか、または追加するかどうか。
| **linesForEditing**             | int32   | テキスト ボックスのサイズ。
| **maxLength**                   | int32   | 値に使用できる最大文字数。
| **textType**                    | 文字列  | 格納されているテキストの種類。 または `richText` のいずれかでなければなりません。 `richText`

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
