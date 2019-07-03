---
author: chackman
ms.author: chackman
title: フォローされたアイテムを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 69657bdc178b153fe1fb5af2a84b6775a01dd129
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436586"
---
# <a name="list-followed-items"></a>フォローされたアイテムを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サインインしているユーザーがフォローされている[アイテム](../resources/driveitem.md)を一覧表示します。
このコレクションには、ユーザーのドライブにあるアイテムと、他のドライブとの間でアクセス可能なアイテムが含まれています。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>応答

このメソッドは、ドライブの所有者がフォローしているアイテムについて、drive [item](../resources/driveitem.md)リソースのコレクションを返します。
アイテムが見つからない場合は、空のコレクションが返されます。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
  ]
}
-->
