---
title: 設定を取得する
description: ユーザーおよび組織の設定 オブジェクトを読み取ります。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64ecf4c4f44cf59bf3c6344edda7510a6997d813
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027077"
---
# <a name="get-settings"></a>設定を取得する

ユーザーおよび組織の[設定](../resources/user-settings.md) オブジェクトを取得します。
[設定](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定を更新する](user-update-settings.md)を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.Read.All、User.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

```http
GET /me/settings/
```

「user id」または「userPrincipalName」を持つリクエストは、ユーザーまたは User.ReadWrite.All 権限を持つユーザーのみがアクセスできます。 詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user-settings.md)設定 オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

