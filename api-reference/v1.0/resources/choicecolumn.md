---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 6841f453cdfd423ead3edeea5895242a28b998f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020829"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn リソースの種類

[columnDefinition ](columndefinition.md)リソースの** choiceColumn **は、選択肢のリストから列の値を選択できることを示します。

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
| **displayAs**      | string             | UX での選択肢の表示方法。 `checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
