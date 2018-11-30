---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 3e61cae016a8ebccae1af59d18c559d6adf63b0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023266"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn リソースの種類

[columnDefinition](columndefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**dateTimeColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名      | 種類               | 説明
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | UX での値の表示方法です。 `default`、`friendly`、`standard` のいずれかでなければなりません。 詳細については、後述します。 指定しない場合、`default` として扱われます。
| **format**         | string             | 値を日付のみで表示するか、日付と時刻で表示するかを示します。 `dateOnly` または `dateTime` のいずれかでなければなりません。

## <a name="displayas-options"></a>DisplayAs オプション

| 値        | 説明
|:-------------|:--------------------------------------------------------------
| **default**  | UX での既定のレンダリングを使用します。
| **friendly** | フレンドリーな相対表現を使用します。(例:  「今日の午後 3:00」)
| **standard** | 標準の絶対表現を使用します。(例:  「2017 年 5 月 10 日、午後 3:20」)


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
