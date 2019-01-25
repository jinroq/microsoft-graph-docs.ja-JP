---
title: 'メッセージ: 購読の取り消し'
description: サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 69d14315fc0732ed12db357f9aa9a0c837f48f29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508826"
---
# <a name="message-unsubscribe"></a>メッセージ: 購読の取り消し

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サイン インユーザーに代わって電子メール要求を送信し、電子メール配布リストから登録を解除します。`List-Unsubscribe` ヘッダー内の情報を使用します。

メッセージの送信者使用できますメーリング リスト ユーザー フレンドリな方法で受信者のオプションを含めることによって脱退します。ように指定することにより、`List-Unsubscribe`次の[RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)各メッセージのメッセージ ヘッダー。

**注** 具体的には、**Unsubscribe** アクションを有効にするには、送信者が URL ベースの登録解除情報ではなく、`mailto:` を指定する必要があります。

そのヘッダーを設定すると、[メッセージ](../resources/message.md) インスタンスの **UnsubscribeEnabled** プロパティが `true` に設定され、**UnsubscribeData** プロパティがヘッダー データに設定されます。

メッセージの **UnsubscribeEnabled** プロパティが `true` の場合、**Unsubscribe** アクションを使用して、メッセージ送信者が管理するとおり、同じような今後のメッセージについてユーザーを登録解除することができます。

**Unsubscribe** アクションが完了すると、メッセージは削除済みアイテム フォルダーに移動します。将来のメール配布からのユーザーの実際の除外は、送信者によって管理されます。

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
| 名前       | 型 | 説明|
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
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
