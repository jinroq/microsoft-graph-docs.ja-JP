---
title: (me) をシングルトンとして定義します。
description: Markdown を確認するためにドキュメントに追加する必要があるのは、次のような点です。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 7c47801cd7c76c201f543587012ba22d34660ee7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730359"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a>ヘルパー (ドキュメントに含まれていない例)

これらはマークダウン スキャナーがグラフ ドキュメントを適切に処理できるようにするため、ドキュメントに追加する必要があったものです。


## <a name="define-the-me-as-singleton"></a>(me) をシングルトンとして定義します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {"blockType": "request", "name": "get_current_user" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-current-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-current-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-current-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-current-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a>ドライブをクエリ可能な entityset として定義します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-from-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-from-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-from-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-from-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a>ユーザーをクエリ可能な entityset として定義します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {"blockType": "request", "name": "get_users" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
