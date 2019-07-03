---
title: 'グループ: subscribeByMail'
description: このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。 Office 365 グループのみをサポートします。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 3ccb84708b9213af4cb883ad79cd81d5f52de4b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442800"
---
# <a name="group-subscribebymail"></a>グループ: subscribeByMail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このメソッドを呼び出すと、現在のユーザーがそのグループ内の新規投稿、イベント、およびファイルに関するメール通知を受信できるようになります。 Office 365 グループのみをサポートします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Prefer | return=minimal. 最小応答ヘッダーが要求ヘッダーに含まれている場合、正常な応答で `204 No Content` コードが返されます。 省略可能。  | 

## <a name="request-body"></a>要求本文

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
#### <a name="request"></a>要求
要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答
応答の例を次に示します。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
