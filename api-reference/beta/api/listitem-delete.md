---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: SharePoint リストからエントリを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 36f0c67dada25128cd1a054c066c1d90ccfcbabb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333494"
---
# <a name="delete-an-item-from-a-list"></a>リストからアイテムを削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[list][] からアイテムを削除します。

[list]: ../resources/list.md

## <a name="permissions"></a>アクセス許可

アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前       | 値 | 説明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="example"></a>例

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a>応答

成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": []
}
-->
