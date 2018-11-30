---
title: IdentityProvider を更新します。
description: 既存の identityProvider プロパティを更新します。
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069175"
---
# <a name="update-identityprovider"></a>IdentityProvider を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

既存の[identityProvider](../resources/identityprovider.md)のプロパティを更新します。

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
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>要求ヘッダー

|名前|説明|
|:---------------|:----------|
|Authorization|ベアラー {トークン}。必須。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>要求本文

要求の本文には、更新する必要がある 1 つまたは複数のプロパティを使用して JSON オブジェクトを提供します。

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|clientId|String|アプリケーションのクライアント ID。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアント ID です。|
|clientSecret|String|アプリケーションのクライアントの機密情報です。 これは、id プロバイダーを持つアプリケーションを登録するときに取得したクライアントの機密情報です。|
|名前|String|Id プロバイダーの表示名。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合、`4xx`について、エラーが返されます。

## <a name="example"></a>使用例

次の例では、トークンの有効期間の**identityProvider**の定義を更新し、組織の既定値として設定します。

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

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
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->