---
title: 設定を取得します。
description: ユーザーと組織の設定オブジェクトを参照してください。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ace7c43b27860832968572628838484bc8c91c84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815492"
---
# <a name="get-settings"></a>設定を取得します。

ユーザーと組織の[設定](../resources/user-settings.md)オブジェクトを参照してください。
[設定](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、[ユーザー設定の更新](user-update-settings.md)を参照してください。

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

'UserPrincipalName' は、ユーザー、または User.ReadWrite.All のアクセス許可を持つユーザーがアクセス可能なや、ユーザー id が要求されます。 詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[ユーザー設定](../resources/user-settings.md)のオブジェクトです。

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

