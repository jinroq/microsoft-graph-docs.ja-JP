---
title: ユーザー用のアプリをインストールする
description: 指定したユーザーの個人スコープにアプリをインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 009d2efe115d8b07f9bdead07965d402db65e65a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908545"
---
# <a name="install-app-for-user"></a>ユーザー用のアプリをインストールする

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[ユーザー](../resources/user.md)の個人スコープに[アプリ](../resources/teamsapp.md)をインストールします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  User.ReadWrite.All、Directory.ReadWrite.All     |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文

要求本文には、追加する既存のカタログアプリの ID が含まれている必要があります。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|teamsApp|String|追加するアプリの ID。|

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
