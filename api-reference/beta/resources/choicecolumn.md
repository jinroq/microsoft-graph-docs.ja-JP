---
author: JeremyKelley
description: columnDefinition リソースの choiceColumn は、選択肢のリストから列の値を選択できることを示します。
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973501"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
