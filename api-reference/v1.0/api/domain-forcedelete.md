---
title: 強制的にドメインを削除する
description: 非同期の長時間実行操作を使用してドメインを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69d95d4189f5660315365420703d3ebb954b9dda
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656651"
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

### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
