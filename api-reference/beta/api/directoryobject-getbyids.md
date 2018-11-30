---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: 選択 ' クエリ オプションはこの操作に使用できません。
ms.openlocfilehash: 87fa774910c1ea6795b6df65ee0f5538d12296bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067402"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>ID のリストからディレクトリ オブジェクトを取得します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。

この関数の一般的な用途は次のとおりです。

* [getMemberObjects](directoryobject-getmemberobjects.md) または [getMemberGroups](directoryobject-getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。
* アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.Read.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター   | 型 |説明|
|:---------------|:--------|:----------|
|ids|String コレクション| オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。 |
|types|String コレクション| 検索するリソースのコレクションのセットを指定するリソースの種類のコレクションです。 指定しない場合、既定では[directoryObject](../resources/directoryobject.md)、すべてのディレクトリで定義されているリソースの種類が含まれています。 派生したオブジェクトは、`directoryObject`コレクションに指定することがあります例:[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、[デバイス](../resources/device.md)、およびようにします。 値は、大文字小文字を区別しません。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>応答

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
