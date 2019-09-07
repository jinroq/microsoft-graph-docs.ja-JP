---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: この操作に ` クエリ オプションは使用できません。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55782b87569b4d153178c604af88126202c88f98
ms.sourcegitcommit: 25884c00cbfa2aa5c001cf777fd0ffa3c9a5ed68
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36758301"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>ID のリストからディレクトリ オブジェクトを取得します。

ID のリストで指定されたディレクトリ オブジェクトを返します。

>[!NOTE]
>ここで返されるディレクトリ オブジェクトは、すべてのプロパティを含む完全なオブジェクトです。 この操作に `$select` クエリ オプションは使用できません。

>[!NOTE]
>この API には[既知](/graph/known-issues#incomplete-objects-when-using-getbyids-request)の問題があります。 返されるすべてのディレクトリ オブジェクトが、すべてのプロパティを含む完全なオブジェクトであるとは限りません。

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

| パラメーター   | 型 |説明|
|:---------------|:--------|:----------|
|ids|String collection| オブジェクトを戻す ID のコレクション。 最大 1000 ID まで指定できます。 |
|types|String コレクション| 検索する一連のリソース コレクションを指定するリソース型のコレクションです。 指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) になります。 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から派生する任意のオブジェクトをコレクションに指定できます。例: [user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) など。 [クラウド ソリューション プロバイダー](https://partner.microsoft.com/ja-JP/cloud-solution-provider) パートナー組織への参照を検索するには、[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0) を指定します。 指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) になります ([クラウド ソリューション プロバイダー](https://partner.microsoft.com/ja-JP/cloud-solution-provider) パートナー組織への参照をのぞく)。 値では、大文字と小文字は区別されません。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求


# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
  "tocPath": "",
  "suppressions": [
  ]
}-->
