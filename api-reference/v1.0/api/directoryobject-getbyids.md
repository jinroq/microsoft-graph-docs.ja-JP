---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: 選択 ' クエリ オプションはこの操作に使用できません。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fab85844d810627ca4e44395477716eb0828ffa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986818"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>ID のリストからディレクトリ オブジェクトを取得します。

ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。

この関数の一般的な用途は次のとおりです。

* [getMemberObjects](directoryobject-getmemberobjects.md) または [getMemberGroups](directoryobject-getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。
* アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.Read.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 種類 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| Content-Type  | string | application/json  |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター   | Type |説明|
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
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
