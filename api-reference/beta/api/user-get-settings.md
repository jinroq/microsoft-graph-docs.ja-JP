---
title: 設定を取得する
description: ユーザーと組織の設定オブジェクトを読み取ります。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dcd9079956b4db8b349ba6b81bd85d8472630643
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334913"
---
# <a name="get-settings"></a>設定を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
GET https://graph.microsoft.com/beta/me/settings
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
