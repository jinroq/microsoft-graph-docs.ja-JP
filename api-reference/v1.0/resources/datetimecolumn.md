---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn リソース型

[columnDefinition](columnDefinition.md) リソースの **dateTimeColumn** は、列の値が日付または時刻であることを示します。

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
| **format**         | string             | 値を日付のみで表示するか、日付と時刻で表示するかを示します。 `dateOnly` または `dateTime` のいずれかでなければなりません

## <a name="displayas-values"></a>DisplayAs 値

| 値        | 説明
|:-------------|:--------------------------------------------------------------
| **default**  | UX での既定のレンダリングを使用します。
| **friendly** | フレンドリな相対表現を使用します。(例:  「今日の午後 3:00」)
| **standard** | 標準の絶対表現を使用します。(例:  「2017 年 5 月 10 日、午後 3:20」)


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
