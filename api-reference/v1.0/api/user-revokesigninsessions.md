---
title: 'ユーザー: revokeSignInSessions'
description: '**SignInSessionsValidFromDateTime** user プロパティを現在の日付と時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1e6f0d737d080314273271063cd970b241366dcc
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450635"
---
# <a name="user-revokesigninsessions"></a>ユーザー: revokeSignInSessions

**SignInSessionsValidFromDateTime** user プロパティを現在の日時にリセットすることによって、ユーザーのアプリケーションに対して発行されたすべての更新トークン (ユーザーのブラウザー内のセッション cookie) を無効にします。 通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。 この操作により、デバイスに依存していないすべてのアプリケーションにユーザーが再度サインインするよう要求することにより、デバイス上のアプリケーション経由で組織のデータにアクセスできなくなります。

>アプリケーションは、無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行すると、アプリケーションはエラーを受け取ります。 このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。

>[!NOTE]
>**RevokeSignInSessions**を呼び出した後、トークンが取り消されるまでに少し時間がかかる場合があります。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | Directory.accessasuser.all、またはすべてのディレクトリを読み取ります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | Directory.ReadWrite.All、Directory.AccessAsUser.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
この操作には、要求コンテンツはありません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

>[!NOTE]
>この API には[既知の問題](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)があります。 このメソッドは、異なる HTTP 応答コードを返します。

## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。

##### <a name="request"></a>要求

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
