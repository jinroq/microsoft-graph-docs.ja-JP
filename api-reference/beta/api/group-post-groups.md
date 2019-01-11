---
title: グループを作成する
description: この API を使用して、要求本文で指定した新しいグループを作成します。次に示す 3 種類のグループのうちの 1 つを作成できます。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 5876c1c327cd1095124675046089a0f8a71a7ca0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887641"
---
# <a name="create-group"></a>グループを作成する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

要求の本体に指定されている新しい[グループ](../resources/group.md)を作成するのにには、この API を使用します。 3 つの種類のグループのいずれかを作成できます。

* Office 365 グループ (統合グループ)
* 動的グループ
* セキュリティ グループ

> **注**:[チーム](../resources/team.md)を作成して、最初にグループを作成し、チームを追加するのには、[チームの作成](../api/team-put-teams.md)を参照してください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
グループを作成するときに指定する[グループ](../resources/group.md)・ リソースのプロパティを次の表に示します。 

| プロパティ | 種類 | 説明|
|:---------------|:--------|:----------|
| displayName | string | アドレス帳に表示するグループの名前。 必須。 |
| mailEnabled | ブール値 | メールが有効なグループの場合は、**true** に設定します。 Office 365 グループを作成する場合**は true**に設定します。 **False**場合は、動的に作成するグループまたはセキュリティ グループを設定します。 必須。 |
| mailNickname | 文字列 | グループの電子メール エイリアス。 必須。 |
| securityEnabled | ブール値 | **真**のセキュリティが有効なグループを設定します。 動的またはセキュリティ グループを作成する場合**は true**に設定します。 Office 365 グループを作成する場合**は false**に設定します。 必須。 |
| owners | string collection | このプロパティは、作成時に、グループの所有者を表します。 省略可能。 |
| メンバー | string collection | このプロパティは、作成時にグループのメンバーを表します。 省略可能。 |

Office 365 グループまたは動的グループを作成している場合は、以下のように **groupTypes** プロパティを指定します。

| グループの種類 | **groupTypes** プロパティ |
|:--------------|:------------------------|
| Office 365 (統合グループともいいます)| "Unified" |
| Dynamic | "DynamicMembership" |
| Security | 設定しない。 |

**グループ**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用すること、`POST`操作し、作成時に実際のデータにカスタム プロパティをグループに追加します。

>**注:** ユーザー コンテキストおよび所有者を指定することがなくプログラムでは、Office 365 のグループを作成すると、匿名で、グループが作成されます。  これを行うと、関連付けられた SharePoint Online サイトで作成されていない自動的にさらに手動で操作が実行されるまでがあります。  

グループの必要に応じて他の書き込み可能なプロパティを指定します。詳細については、[group](../resources/group.md) リソースのプロパティをご覧ください。

## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。

## <a name="example"></a>例
#### <a name="request-1"></a>要求 1
例の最初の要求では、Office 365 グループを作成します。
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response"></a>応答
応答の例を次に示します。
>**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>要求 2
2 番目の例の要求では、所有者が指定されている、Office 365 のグループを作成します。
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json
 {
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a>応答 2
次は、正常な応答の例です。
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
 {
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
