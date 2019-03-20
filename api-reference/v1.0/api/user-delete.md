---
title: ユーザーを削除する - Microsoft Graph API
description: Microsoft Graph API (REST) のユーザー リソース (エンティティ) の削除方法について説明します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba27c81e5cb6b8bc8738c419b467e686932bc7c8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258066"
---
# <a name="delete-a-user"></a>ユーザーを削除する

ユーザーを削除します。  

ユーザー リソースを削除すると、一時的なコンテナーに移動され、30 日以内であれば復元できます。  それ以降、これらのユーザーは完全に削除されます。  詳細については、「[deletedItems](../resources/directory.md)」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値|
|:-----------|:------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例

## <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
### <a name="response"></a>応答

以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
