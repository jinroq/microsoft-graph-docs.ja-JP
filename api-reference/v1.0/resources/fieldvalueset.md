---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: FieldValueSet
ms.openlocfilehash: dfe11b4cdf095e8878da54760032d788f97756fb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="fieldvalueset-resource"></a>FieldValueSet リソース

[listItem](listItem.md) リソースでの列の値を表します。

## <a name="json-representation"></a>JSON 表記

以下は、**fieldValueSet** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a>プロパティ

**listItem** の各ユーザーに表示されるフィールドは、**fieldValueSet** の名前と値のペアとして返されます。
上記の例は、**Author**、**Name**、**Color**、**Quantity** の 4 つの列を含むリストを示しています。

既定では、ルックアップ フィールド (上記の `Author` など) は返されません。
代わりにサーバーは、ルックアップの対象となる listItem を参照する 'LookupId' フィールド (上記の `AuthorLookupId` など) を返します。
'LookupId' フィールドの名前は元のフィールド名の末尾に `LookupId` を付けたものです。

1 つのクエリでは、ルックアップ フィールドを最大 12 個まで要求できます。
サーバーは、要求に `select` ステートメントと必要なフィールドが含まれていると、ルックアップ値を返します。
例:

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

1 つのクエリでは、最大 12 個のルックアップ フィールドと、任意の数の通常のフィールドを要求できます。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
