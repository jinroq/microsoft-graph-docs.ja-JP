---
title: identityProvider を作成する
description: 表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい  identityProvider  を作成します。
localization_priority: Normal
ms.openlocfilehash: 5d9940803ab9a140312c21f21832623eccd77969
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323851"
---
# <a name="create-identityprovider"></a>identityProvider を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示名、identityProvider の種類、クライアント ID、クライアント シークレットを指定して、新しい [ identityProvider ](../resources/identityprovider.md) を作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)|IdentityProvider.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)| サポートされていません。|
|アプリケーション|サポートされていません。|

職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a>要求ヘッダー

|名前|説明|
|:---------------|:----------|
|Authorization|ベアラー {トークン}。必須。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>要求本文

要求本文で、[identityProvider](../resources/identityprovider.md) オブジェクトの JSON 表記を提供します。 次の表に示す、すべてのプロパティが必要です。

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|clientId|String|アプリケーションのクライアント ID。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。|
|clientSecret|String|アプリケーションでのクライアント シークレット。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。|
|name|String|ID プロバイダーの表示名。|
|type|String|ID プロバイダーの型。 次のいずれかの値であることが必要です。 <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [identityProvider](../resources/identityprovider.md) オブジェクトを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例

次の例では、**identityProvider** を作成します。

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
