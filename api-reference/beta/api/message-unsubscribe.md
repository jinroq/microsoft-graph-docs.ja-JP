---
title: 'メッセージ: 購読の取り消し'
description: サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。
author: angelgolfer-ms
ms.openlocfilehash: e516a8aa68bde02f056e503da9c85d4e7a6f62fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357226"
---
# <a name="message-unsubscribe"></a>メッセージ: 購読の取り消し

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。

メッセージの送信者使用できますメーリング リスト ユーザー フレンドリな方法で受信者のオプションを含めることによって脱退します。ように指定することにより、`List-Unsubscribe`次の[RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)各メッセージのメッセージ ヘッダー。

**メモ**具体的には、**購読の取り消し**操作をするため動作、送信者を指定してください`mailto:`し、URL ベースではない情報の購読を解除します。

そのヘッダーを設定する[メッセージ](../resources/message.md)のインスタンスの**unsubscribeEnabled**プロパティを設定します`true`、 **unsubscribeData**プロパティは、ヘッダーのデータをします。

かどうか、メッセージの**unsubscribeEnabled**プロパティは、 `true`、メッセージの送信者によって管理のようなメッセージからユーザーの購読を解除する**購読を解除**アクションを使用することができます。

成功を**登録解除**の操作は、メッセージを**削除済みアイテム**フォルダーに移動します。 将来のメールの配信から、ユーザーの実際の除外は、送信者によって管理されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.Send    |
|委任 (個人用 Microsoft アカウント) | Mail.Send    |
|アプリケーション | Mail.Send |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a>応答
以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
