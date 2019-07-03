---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをチェックインする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 84958a6dcbadb0b92d7a25bfb36bb53edbd3189a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436523"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a>DriveItem リソースへの変更をチェックインする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。


|   名前    | 値  |                                                説明                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| checkInAs | string | 省略可能。 チェックイン操作が完了した後のドキュメントの適切なステータス。 `published` または未設定となります。 |
| comment   | string | バージョンに関連付けられているチェックイン コメント。                                                   |

## <a name="example"></a>例

この例では、`{item-id}` で識別されるファイルをチェックインします。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No content` を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a>備考


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
