---
title: ProfilePhoto を更新する
description: サインイン ユーザー、または指定されたグループあるいは連絡先を含むテナント内の任意のユーザーの写真を更新します。 存在するため
localization_priority: Normal
ms.openlocfilehash: 1cf4d99f55768a6fad868d91d526fc5fd0b7b5ca
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332065"
---
# <a name="update-profilephoto"></a>ProfilePhoto を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サインイン ユーザー、または指定されたグループあるいは連絡先を含むテナント内の任意のユーザーの写真を更新します。現在各 REST 要求の合計サイズは 4 MB に制限されているため、追加する写真のサイズは 4 MB 未満に制限されます。

ベータ版では、この操作に PUT のみを使用します。

> **注** ベータ版の写真更新操作では、ユーザーの職場用または学校用メールボックスのみがサポートされ、個人用メールボックスはサポートされていません。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | サインインしている**ユーザー**のプロファイル写真:<br/>ユーザー読み取り/書き込みユーザー。<br /><br />**group** リソースの場合:<br />Group.ReadWrite.All<br /><br />**contact** リソースの場合:<br />Contacts.ReadWrite |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | **user** リソースの場合:<br/>User.ReadWrite.All<br /><br />**group** リソースの場合:<br />Group.ReadWrite.All<br /><br />**contact** リソースの場合:<br />Contacts.ReadWrite |

> **メモ**組織内のユーザーの写真を更新するには、アプリに、ユーザーの代わりに使用するのではなく、アプリケーションのすべてのアクセス許可を持ち、独自の id でこの API を呼び出す必要があります。 詳細については、「サインインして[いるユーザーなしでアクセスを取得](/graph/auth-v2-service)する」を参照してください。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | image/jpeg。必須。  |

## <a name="request-body"></a>要求本文
要求本文に、写真のバイナリ データを含めます。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
