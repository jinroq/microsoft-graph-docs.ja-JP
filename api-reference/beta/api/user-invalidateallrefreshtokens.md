---
title: 'ユーザー: invalidateAllRefreshTokens'
description: '**Refreshtokensvalidfromdatetime**ユーザープロパティを現在の日付/時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。 通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。  この操作を実行すると、ユーザーが最初にサインインする必要がなく、デバイス上のアプリケーションを介してアクセスされる組織のデータにアクセスできなくなります。 実際、この操作を実行すると、デバイスに関係なく、以前に同意していたすべてのアプリケーションに対して、ユーザーが再度サインインすることになります。'
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6146285b0fa6e2fb7c8cabde1f96d22e4f897e4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362370"
---
# <a name="user-invalidateallrefreshtokens"></a>ユーザー: invalidateAllRefreshTokens

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Refreshtokensvalidfromdatetime**ユーザープロパティを現在の日付/時刻にリセットすることによって、アプリケーションに発行されたすべてのユーザーの更新トークン (およびユーザーのブラウザー内のセッション cookie) を無効にします。 通常、この操作は (ユーザーまたは管理者によって) ユーザーが紛失または盗難したデバイスを持っている場合に実行されます。  この操作を実行すると、ユーザーが最初にサインインする必要がなく、デバイス上のアプリケーションを介してアクセスされる組織のデータにアクセスできなくなります。 実際、この操作を実行すると、デバイスに関係なく、以前に同意していたすべてのアプリケーションに対して、ユーザーが再度サインインすることになります。

開発者にとって、アプリケーションが無効にされた更新トークンを使用して、このユーザーの代理アクセストークンの引き換えを試行した場合、アプリケーションでエラーが発生します。 このような場合、アプリケーションは承認エンドポイントに対して要求を行うことで新しい更新トークンを取得する必要があります。これにより、ユーザーは強制的にサインインできるようになります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

+ アプリケーションで、サインインしているユーザーが同意のアプリケーションを無効にできるようにするには、Directory.accessasuser.all のようにします。
+ 管理者が同意、Directory.accessasuser.all のいずれかのユーザーがアプリケーションを無効にすることを許可するアプリケーションの場合。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
この操作には、要求コンテンツはありません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
以下は、応答の例です。 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
