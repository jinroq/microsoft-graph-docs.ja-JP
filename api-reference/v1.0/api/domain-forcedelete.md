---
title: 強制的にドメインの削除
description: 非同期実行時間の長い操作を使用してドメインを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbf56fdd2f623a918b43298626bd08269ad922ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918428"
---
# <a name="force-domain-deletion"></a>強制的にドメインの削除

非同期実行時間の長い操作を使用してドメインを削除します。

次の操作は、この操作の一部として実行されます。

* 更新、 `userPrincipalName`、 `mail`、および`proxyAddresses`のプロパティ`users`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。

* 更新、`mail`の`groups`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。

* 更新、`identifierUris`の`applications`初期 onmicrosoft.com ドメインを使用する削除されたドメインへの参照にします。

* 名前を変更するオブジェクトの数が 1000 を超える場合は、エラーが返されます。

* 1 つの場合の`applications`は、マルチ テナント アプリケーションの名前を変更するのには、エラーが返されます。

ドメインの削除が完了すると、削除されたドメインの API 操作は HTTP 404 ステータス コードを返します。 ドメインの削除を確認するには、[ドメインの取得](domain-get.md)の操作を行うことができます。

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
|`disableUserAccounts`|`Boolean`| 名前を変更するユーザー アカウントを無効にするオプションです。 ユーザー アカウントを無効にすると、ユーザーはサインインするのには使用できません。 場合**は true**に設定、`users`この操作の一部が無効にするたびに更新します。  既定値は**true**です。 |

## <a name="response-body"></a>応答本文

かどうかは成功すると、このメソッドを返します`HTTP/1.1 204 OK`ステータス コードです。

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
