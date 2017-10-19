---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn リソースの種類

[columnDefinition](columnDefinition.md) リソースの **choiceColumn** は、選択肢のリストから列の値を選択できることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**choiceColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名      | 種類               | 説明
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | boolean            | true の場合、設定された選択肢にないカスタム値を使用できます。
| **choices**        | collection(string) | この列に使用可能な値のリスト。
| **displayAs**      | string             | UX での選択肢の表示方法。 `checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
