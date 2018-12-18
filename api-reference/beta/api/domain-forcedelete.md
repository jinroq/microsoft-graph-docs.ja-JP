---
title: 'ドメイン: forceDelete'
description: 非同期操作を使用してドメインを削除します。
author: lleonard-msft
ms.openlocfilehash: 4af5b70fca7600538d4212768243d8de82eb79ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316213"
---
# <a name="domain-forcedelete"></a>ドメイン: forceDelete

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

非同期操作を使用してドメインを削除します。

次の操作は、この操作の一部として実行されます。

* UPN、EmailAddress、および削除されたドメインへの参照を持つユーザーのメタベースを変更します。

* 削除したドメインへの参照を持つグループの電子メール アドレスの名前を変更します。

* 削除したドメインへの参照を持つアプリケーションの identifierUris の名前を変更します。

* 名前を変更するオブジェクトの数が 1000 を超える場合は、エラーが返されます。

* マルチ テナント アプリケーションの名前を変更するアプリケーションのいずれかの場合は、エラーが返されます。

ドメインの削除が完了すると、API の操作、削除されたドメインの HTTP 応答コード 404 が返されます。 ドメインの削除を確認するには、[ドメインを取得](domain-get.md)を実行できます。 ドメインが正常に削除された場合の応答で 404 の HTTP 応答コードが返されます。

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

| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。|
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 種類   |説明|
|:---------------|:--------|:----------|
|disableUserAccounts|ブール型| 名前を変更したユーザー アカウントを無効にするオプションです。 ユーザー アカウントを無効にすると、ユーザーはサインインするのには使用できません。<br>*場合は true。*(デフォルト) - ユーザーがこの操作の一部として名前が変更されたアカウントが無効になります。<br>*False* - この操作の一部として名前を変更するユーザー アカウントは無効になっていません。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。 

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
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