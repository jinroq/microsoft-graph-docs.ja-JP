---
title: 'user: checkMemberObjects'
description: 指定したユーザーオブジェクトのグループ、ディレクトリの役割、または管理単位オブジェクトの一覧のメンバーシップを確認します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 654208a1163e2d99c0685d72588d64d9b0bf228f
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853871"
---
# <a name="user-checkmemberobjects"></a>user: checkMemberObjects

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したユーザーオブジェクトのグループ、ディレクトリの役割、または管理単位オブジェクトの一覧のメンバーシップを確認します。 このメソッドは推移的です。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | ReadBasic、user。すべてのユーザーが読み取ります。<br><br>さらに、次の機能も使用できます。<br><br><ul><li>グループ内のメンバーシップを確認する場合: groups、すべて。</li><li>管理単位でのメンバーシップを確認する場合: AdministrativeUnit、AdministrativeUnit。</li><li>ディレクトリロールのメンバーシップを確認している場合: RoleManagement、RoleManagement</li></ul>Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | すべてのユーザーを取得します。すべてのユーザーに対して。<br>そして：<ul><li>グループ内のメンバーシップを確認する場合: groups、すべて。</li><li>管理単位でのメンバーシップを確認する場合: AdministrativeUnit、AdministrativeUnit。</li><li>ディレクトリロールのメンバーシップを確認している場合: RoleManagement、RoleManagement</li></ul>Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
|:--------------|:--------------|
| Authorization | ベアラー {トークン} |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型        | 説明 |
|:-------------|:------------|:------------|
|ids|String collection|メンバーシップを確認するために、ディレクトリの役割のグループ、ディレクトリの役割、管理単位、または roleTemplate Id のオブジェクト Id を含むコレクション。 最大20個のオブジェクトを指定できます。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で新しい文字列コレクションオブジェクトを返します。

## <a name="examples"></a>例

この API を呼び出す方法の例を次に示します。

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a>応答

応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
