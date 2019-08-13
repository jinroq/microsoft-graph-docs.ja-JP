---
title: OAuth2PermissionGrant の更新
description: OAuth2PermissionGrant オブジェクトのプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec040d8a645c37bfd80f25ce66e3947e4256759e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346783"
---
# <a name="update-oauth2permissiongrant"></a>OAuth2PermissionGrant の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth2PermissionGrant オブジェクトのプロパティを更新します。

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
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|scope|String| OAuth 2.0 アクセストークンでリソースアプリケーションが想定するスコープ要求の値を指定します。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
