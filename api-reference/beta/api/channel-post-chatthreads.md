---
title: チャットのスレッドを作成します。
description: ルート メッセージを指定することによって、指定されたチャネルでチャットの新しいスレッドを作成します。
ms.openlocfilehash: 9a2a35a086c6689d1b76a56b70cd3637ec23c3a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066686"
---
# <a name="create-chat-thread"></a>チャットのスレッドを作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ルート メッセージを指定することによって、指定された[チャネル](../resources/channel.md)でチャットの新しいスレッドを作成します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

> 現在、[委任されたアクセス許可](/graph/permissions-reference)をのみがこの操作に対してサポートされています。  将来のリリースでは、アプリケーションのアクセス許可をサポートします。 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求の本文に rootMessage プロパティが含まれている[chatThread](../resources/chatthread.md)オブジェクトの JSON の形式を指定します。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`、空の応答の本体を含む応答コード。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> 現時点では、文字列ではなく整数として、コンテンツ タイプを指定する必要があります:"text"または"html"の場合は 1 の場合は 0 です。  API の将来のリリースには、これを修正します。

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
