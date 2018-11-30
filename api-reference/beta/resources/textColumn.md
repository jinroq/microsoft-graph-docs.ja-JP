---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 5ff280b6c969d9832e2f81f77dc32237f9905aad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069970"
---
# <a name="textcolumn-resource-type"></a>TableColumn リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ名                   | 型   | 説明
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | 文字列 | 複数行のテキストを許可するかどうか。
| **appendChangesToExistingText** | 文字列 | この列への更新が既存のテキストを置き換えるか、または追加するか。
| **linesForEditing**             | int    | テキスト ボックスのサイズ。
| **maxLength**                   | int    | 値に使用できる最大文字数。
| **textType**                    | 文字列 | 格納されているテキストの種類。 `plain` または `richText` のいずれかでなければなりません。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
