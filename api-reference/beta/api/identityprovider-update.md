---
title: identityProvider を更新する
description: '既存の identityprovider.readwrite.all: のプロパティを更新します。'
localization_priority: Normal
ms.openlocfilehash: d98bc5d0bd7a8f165f33c89548a69805039cdf07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501463"
---
# <a name="update-identityprovider"></a>identityProvider を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
