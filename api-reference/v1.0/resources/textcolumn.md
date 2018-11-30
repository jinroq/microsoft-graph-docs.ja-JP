---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 810554620e747d3160a6d8c74913518b8590c19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023480"
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
| **allowMultipleLines**          | ブール | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | ブール | この列への更新が既存のテキストを置き換えるか、または追加するか。
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
