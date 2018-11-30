---
title: '参加者: muteAll'
description: 呼び出しのすべての参加者をミュートします。
ms.openlocfilehash: f0da6f44801559fe7258d61fff9d5c87cc606702
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067479"
---
# <a name="participant-muteall"></a>参加者: muteAll

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

呼び出しのすべての参加者をミュートします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | サポート対象外                               |
| 委任 (個人用 Microsoft アカウント) | サポート対象外                               |
| アプリケーション                            | なし                                        |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a>要求ヘッダー
| 名前          | 説明               |
|:--------------|:--------------------------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター      | 型    |説明|
|:---------------|:--------|:----------|
|participants|String コレクション|参加者をミュートします。|
|clientContext|String|クライアントのコンテキスト。|

## <a name="response"></a>応答
かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[commsOperation](../resources/commsoperation.md)のオブジェクトです。

## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求
次の例は要求を示しています。
<!-- {
  "blockType": "request",
  "name": "participant_muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a>応答

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
