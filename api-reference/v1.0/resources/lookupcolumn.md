---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 73d372d52447906c826d79e3c614635a3023cefa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022835"
---
# <a name="lookupcolumn-resource-type"></a>LookupColumn リソースの種類

[columnDefinition](columndefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。

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
| **primaryLookupColumnId** | string  | 指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト項目から、新たに追加されたフィールドを取り出します。 *プライマリ*によって検索されたリスト項目を、ここで指定された列のソースとして使用します。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
