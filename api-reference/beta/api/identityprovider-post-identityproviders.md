---
title: IdentityProvider を作成します。
description: 新しい identityProvider を作成するには、表示名、identityProvider の種類、クライアント ID とクライアント シークレットを指定します。
localization_priority: Normal
ms.openlocfilehash: 50ead5acbbda7725e44de55865d6fe2184c89647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866235"
---
# <a name="create-identityprovider"></a>IdentityProvider を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

新しい[identityProvider](../resources/identityprovider.md)を作成するには、表示名、identityProvider の種類、クライアント ID とクライアント シークレットを指定します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)|IdentityProvider.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)| サポートされていません。|
|アプリケーション|サポートされていません。|

職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。

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

要求の本文には、 [identityProvider](../resources/identityprovider.md)オブジェクトの JSON 表現を提供します。 次の表に記載されているすべてのプロパティは、必要があります。

|プロパティ|種類|説明|
|:---------------|:--------|:----------|
|clientId|String|アプリケーションのクライアント ID。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。|
|clientSecret|String|アプリケーションのクライアントの機密情報です。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。|
|名前|String|Id プロバイダーの表示名。|
|type|String|Id プロバイダーの種類。 次の値のいずれかを指定する必要があります。 <ul><li/>Microsoft<li/>Google<li/>アマゾン<li/>LinkedIn<li/>Facebook</ul>|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[identityProvider](../resources/identityprovider.md)のオブジェクトです。 失敗した場合、`4xx`について、エラーが返されます。

## <a name="example"></a>例

次の使用例は、 **identityProvider**を作成します。

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
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
