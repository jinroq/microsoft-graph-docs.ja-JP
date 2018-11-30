---
title: 'ユーザー: invalidateAllRefreshTokens'
description: '**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。 通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。  この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。 実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。'
ms.openlocfilehash: 23743c4bc372193a5478d79432b7bb4e0a9ec4ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073223"
---
# <a name="user-invalidateallrefreshtokens"></a>ユーザー: invalidateAllRefreshTokens

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることでアプリケーション (と同様に、ユーザーのブラウザーでセッション cookie) を発行したユーザーの更新のトークンのすべてを無効にします。 通常、この操作は、ユーザーが紛失または盗難に遭ったデバイスを持っている場合、(ユーザーまたは管理者) によって実行されます。  この操作は、任意のユーザーが最初に、もう一度サインインする必要がないデバイス上のアプリケーションを通じてアクセスされる組織のデータにアクセスをできなくなります。 実際には、この操作は強制的にもう一度サインインして、以前に、配信されるすべてのアプリケーションのユーザーは、デバイスに依存しません。

開発者は、アプリケーションによって、無効な更新トークンを使用してこのユーザーの委任されたアクセス トークンを償還しようとする場合、アプリケーション エラーが表示されます。 このような場合は、アプリケーションが承認の端点にサインインするユーザーを強制的に実行を要求することによって、新しい更新のトークンを取得する必要があります。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

+ アプリケーションを無効にするユーザーに、署名を許可するアプリケーションに同意した: User.ReadWrite、Directory.ReadWrite.All、Directory.AccessAsUser.All
+ 同意したユーザーのアプリケーションを無効にする管理者を許可するアプリケーション: Directory.ReadWrite.All、Directory.AccessAsUser.All

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
この操作には、要求のコンテンツがありません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

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
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
