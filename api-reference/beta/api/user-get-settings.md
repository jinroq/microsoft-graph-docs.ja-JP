---
title: 設定を取得する
description: ユーザーと組織の設定オブジェクトを読み取ります。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536576"
---
# <a name="get-settings"></a>設定を取得する

ユーザーと組織の[設定](../resources/user-settings.md)オブジェクトを読み取ります。
[settings](../resources/user-settings.md)オブジェクトのプロパティを更新する方法については、「[ユーザーの設定を更新](user-update-settings.md)する」を参照してください。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | User.Read.All、User.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | user。すべてのユーザーを取得します。 |

## <a name="http-request"></a>HTTP 要求

```http
GET /me/settings/
```

' user id ' または ' userPrincipalName ' を持つ要求は、ユーザーまたはすべてのアクセス許可を持つユーザーのみがアクセスできます。 詳細については、「 [Permissions](/graph/permissions-reference)」を参照してください。

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[ユーザー設定](../resources/user-settings.md)オブジェクトを返します。

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

