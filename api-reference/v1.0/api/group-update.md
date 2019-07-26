---
title: グループを更新する
description: グループ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 76adffb439e8e2abbfedfa9ac23e840660977443
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885324"
---
# <a name="update-group"></a>グループを更新する

グループ オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。|
|autoSubscribeNewMembers|Boolean|既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。|
|description|String|グループに関するオプションの説明。 |
|displayName|String|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。 |
|groupTypes|String collection|グループの種類とそのメンバーシップを指定します。  <br><br>コレクションに **Unified** が含まれている場合、そのグループは Office 365 グループです。それ以外の場合はセキュリティ グループです。  <br><br>コレクションに **DynamicMembership** が含まれている場合、そのグループには動的メンバーシップがあります。それ以外の場合は、メンバーシップは静的です。 |
|mailEnabled|ブール値|メールが有効なグループであるかどうかを指定します。|
|mailNickname|文字列|グループの電子メール エイリアス。 このプロパティは、グループの作成時に指定する必要があります。 |
|securityEnabled|ブール値|グループがセキュリティ グループであるかどうかを指定します。 |
|visibility|String|Office 365 グループの表示を指定します。 可能な値は以下のどれかです: **Private**、**Public**または empty (これは **Public**と解釈されます)。|

> **注意:** 
>
> - 上記の表に他のプロパティを含めずに、独自のPATCHリクエストで指定して**autoSubscribeNewMembers**を更新することができます。
> - コア グループの管理とマネージメントに関するグループ API のサブセットのみが、アプリケーションのアクセス許可と委任されたアクセス許可をサポートします。**autoSubscribeNewMembers** の更新を含む他のすべてのグループ API のメンバーは、委任されたアクセス許可のみをサポートします。例については、「[既知の問題](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes)」を参照してください。
> - Microsoft Exchange Server でメールが有効なセキュリティ グループを更新するためのルールが複雑になる場合があります。詳細については、「[Exchange Server でメールが有効なセキュリティ グループを管理する](https://docs.microsoft.com/ja-JP/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)」を参照してください。


## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

次の例は、グループを作成する方法を示しています。

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
