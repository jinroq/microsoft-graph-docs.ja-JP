---
title: user の作成
description: この API を使用して、新しいユーザーを作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5efcc4bd793ca876d1db5860785c3ba67d447ade
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637123"
---
# <a name="create-user"></a>ユーザーを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この API を使用して、新しいユーザーを作成します。要求本文には、作成するユーザーが含まれています。少なくとも、ユーザーに必要なプロパティを指定する必要があります。必要に応じて、その他の書き込み可能なプロパティを指定することもできます。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。

次の表に、ユーザーの作成時に必要になるプロパティを示します。

| パラメーター | 型 | 説明|
|:---------------|:--------|:----------|
|accountEnabled |boolean |アカウントが有効な場合は true。それ以外の場合は false。|
|displayName |string |ユーザーのアドレス帳に表示される名前。|
|onPremisesImmutableId |string |ユーザーの userPrincipalName (UPN) プロパティにフェデレーション ドメインを使用している場合は、新しいユーザー アカウントの作成時にのみ指定する必要があります|
|mailNickname |string |ユーザーのメール エイリアス。|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md) |ユーザーのパスワード プロファイル。|
|userPrincipalName |string |ユーザー プリンシパル名 (someuser@contoso.com)。|

**ユーザー**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`POST` 、操作を使用して、作成中にユーザーインスタンスにカスタムプロパティを追加することができます。

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
要求本文で、[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_user_from_users_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
