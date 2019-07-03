---
title: 'メッセージ: forward'
description: 'メッセージを転送する、コメントを追加する、または更新可能なプロパティを変更する  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e51c108fd4f21df112f65edbe9af0fe879d4b304
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448055"
---
# <a name="message-forward"></a>メッセージ: forward

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メッセージを転送する、コメントを追加する、または更新可能なプロパティを変更する  
すべて1回の**転送**呼び出し。 メッセージは [送信済みアイテム] フォルダーに保存されます。

または、最初に[下書きの転送メッセージを作成して](../api/message-createforward.md)コメントを含めるか、メッセージのプロパティを更新し、転送メッセージを[送信](../api/message-send.md)します。

**注**

- パラメーターには、comment または body プロパティのいずれかを指定できます。 **** `message` 両方を指定すると、「HTTP 400 要求が正しくありません」というエラーが返されます。
- パラメーターを指定するか`toRecipients` 、 `message`パラメーターの**トーラス**プロパティを指定する必要があります。 両方を指定するか、どちらも指定しないと、「HTTP 400 要求が正しくありません」というエラーが返されます。

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
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type | string  | エンティティ本文内のデータの性質です。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|comment|String|含めるコメントです。空の文字列にすることができます。|
|toRecipients|[recipient](../resources/recipient.md) collection|受信者の一覧です。|
|message|[message](../resources/message.md)|返信メッセージで更新する書き込み可能なプロパティです。|

## <a name="response"></a>応答

成功した場合、このメソッドは `202 Accepted` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
次の例では、 **isDeliveryReceiptRequested**プロパティを true に設定し、コメントを追加してメッセージを転送します。
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
<!--
{
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
