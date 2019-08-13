---
title: identityProvider を更新する
description: 既存の identityProvider のプロパティを更新する
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4a1bd498f1f0ee6501174d85673d9b60e93a07b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369886"
---
# <a name="update-identityprovider"></a>identityProvider を更新する

既存の [identityProvider](../resources/identityprovider.md) のプロパティを更新する。

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
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>要求ヘッダー

|名前|説明|
|:---------------|:----------|
|Authorization|ベアラー {トークン}。必須。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>要求本文

要求本文で、更新が必要なプロパティを 1 つまたは複数持つ JSON オブジェクトを提供します。

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|clientId|String|アプリケーションのクライアント ID。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント ID です。|
|clientSecret|String|アプリケーションでのクライアント シークレット。 アプリケーションを ID プロバイダーに登録した際に取得したクライアント シークレットです。|
|name|String|ID プロバイダーの表示名。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例

次の例では、トークンの有効期間の定義 **identityProvider** を更新し、それを組織の既定値として設定します。

##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
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
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
