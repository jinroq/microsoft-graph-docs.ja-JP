---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a48ad30e2610ea13a5859ce8f4f224dab8af5011
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987147"
---
# <a name="update-an-item-in-a-list"></a>リスト内のアイテムを更新する

**[listItem][]** のプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前       | 値 | 説明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。


## <a name="request-body"></a>要求本文

要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。

## <a name="example"></a>例

ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。
listItem の他の値はすべてそのままです。 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a>応答

成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
