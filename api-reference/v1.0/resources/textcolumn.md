---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a>TextColumn リソースの種類

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

| プロパティ名                   | 種類   | 説明
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | string | この列への更新により、既存のテキストを置き換えるか、既存のテキストに追加するか。
| **linesForEditing**             | int    | テキスト ボックスのサイズ。
| **maxLength**                   | int    | 値に使用できる最大文字数。
| **textType**                    | string | 格納されているテキストの種類。 `plain` または `richText` のいずれかでなければなりません

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
