---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn リソースの種類

[columnDefinition](columnDefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。

## <a name="json-representation"></a>JSON 表記

以下は、**lookupColumn** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名             | 種類    | 説明
|:--------------------------|:--------|:---------------------------------------
| **allowMultipleValues**   | boolean | ソースから複数の値を選択できるかどうかを示します。
| **allowUnlimitedLength**  | boolean | 列の値が標準の 255 文字の制限を超えることができるかどうかを示します。
| **columnName**            | string  | 検索元の列の名前。
| **listId**                | string  | 検索元リストの一意識別子。
| **primaryLookupColumnId** | string  | 指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト アイテムから、新たに追加されたフィールドを取り出します。 *プライマリ*によって検索されたリスト アイテムを、ここで指定された列のソースとして使用します。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
