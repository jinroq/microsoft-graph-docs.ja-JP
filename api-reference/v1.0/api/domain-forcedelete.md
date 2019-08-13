---
title: 強制的にドメインを削除する
description: 非同期の長時間実行操作を使用してドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35f2ec6ff71e9668a7774f96acfc5ed383de076c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375318"
---
# <a name="force-domain-deletion"></a>強制的にドメインを削除する

非同期の長時間実行操作を使用してドメインを削除します。

この操作の一部として、次のアクションが実行されます。

* 最初の`userPrincipalName`onmicrosoft.com `mail`ドメインを`proxyAddresses`使用する`users`ために、削除されたドメインへの参照で、、、およびのプロパティを更新します。

* の`mail` `groups`プロパティを、削除されたドメインへの参照で更新して、最初の onmicrosoft.com ドメインを使用します。

* の`identifierUris` `applications`プロパティを、削除されたドメインへの参照で更新して、最初の onmicrosoft.com ドメインを使用します。

* 名前を変更するオブジェクトの数が1000より大きい場合は、エラーが返されます。

* 名前`applications`を変更する1つのがマルチテナントアプリの場合は、エラーが返されます。

ドメイン削除の完了後、削除されたドメインの API 操作は HTTP 404 状態コードを返します。 ドメインの削除を確認するには、ドメインの[取得](domain-get.md)操作を実行します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> {Id} には、ドメインを完全修飾ドメイン名で指定します。

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型 | 説明 |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| 名前が変更されたユーザーアカウントを無効にするオプション。 ユーザーアカウントが無効になっている場合、ユーザーはサインインすることができません。 **True**に設定すると`users` 、この操作の一部として更新されたものは無効になります。  既定値は **true** です。 |

## <a name="response-body"></a>応答本文

成功した場合、この`HTTP/1.1 204 OK`メソッドは状態コードを返します。

## <a name="example"></a>例

### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
