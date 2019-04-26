---
title: 'ドメイン: forcedelete'
description: 非同期操作を使用してドメインを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c58b7d345ba7c5cdc7c029ecf929676fc7529f12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325925"
---
# <a name="domain-forcedelete"></a>ドメイン: forcedelete

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

非同期操作を使用してドメインを削除します。

この操作の一部として、次のアクションが実行されます。

* UPN、EmailAddress、および ProxyAddress のユーザーの名前を、削除されたドメインへの参照に変更します。

* 削除されたドメインへの参照を使用して、グループの EmailAddress の名前を変更します。

* アプリケーションの identifieruris の名前を、削除されたドメインへの参照に変更します。

* 名前を変更するオブジェクトの数が1000より大きい場合は、エラーが返されます。

* 名前を変更するアプリケーションのいずれかがマルチテナントアプリの場合は、エラーが返されます。

ドメイン削除の完了後、削除されたドメインの API 操作は 404 HTTP 応答コードを返します。 ドメインの削除を確認するには、 [get ドメイン](domain-get.md)を実行します。 ドメインが正常に削除された場合は、応答で 404 HTTP 応答コードが返されます。

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

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|disableuseraccounts|Boolean| 名前の変更されたユーザーアカウントを無効にするオプション。 ユーザーアカウントが無効になっている場合、ユーザーはサインインすることができません。<br>*True*(既定値)-この操作の一部として名前が変更されたユーザーアカウントは無効になります。<br>*False* -この操作の一部として名前が変更されたユーザーアカウントは無効になりません。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
