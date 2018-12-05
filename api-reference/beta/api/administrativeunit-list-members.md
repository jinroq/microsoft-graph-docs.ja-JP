---
title: メンバーを一覧表示する
description: この API を使用して、メンバーを取得する] ボックスの一覧 (ユーザーおよびグループ) の管理単位です。
ms.openlocfilehash: c2d86992ccffd9d0ec4df90f5209ed5d6881ed16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069296"
---
# <a name="list-members"></a>メンバーを一覧表示する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

この API を使用して、メンバーを取得する] ボックスの一覧 (ユーザーおよびグループ) の管理単位です。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.Read.All、Directory.ReadWrite.All |

> 注: 非表示のメンバーシップの管理単位のメンバーを列挙するには、Member.Read.Hidden アクセス許可が必要です。

## <a name="http-request"></a>HTTP 要求

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[ユーザー](../resources/user.md)または[グループ](../resources/group.md)のオブジェクトのコレクションです。  代わりに、配置する場合は、`$ref`の応答には要求の最後のコレクションが含まれて`@odata.id`メンバーへのリンクと Url です。

## <a name="examples"></a>例
##### <a name="list-member-objects"></a>メンバー オブジェクトのリスト
次のような要求には、ユーザーおよびグループのコレクションを取得、管理単位のメンバーが表示されます。

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a>リストのメンバーの参照
次のような要求には、メンバーの参照のコレクションを取得、管理単位が一覧表示`@odata.id`メンバーへの参照。
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```