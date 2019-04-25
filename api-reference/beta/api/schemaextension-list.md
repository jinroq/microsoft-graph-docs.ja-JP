---
title: schemaExtensions を一覧表示する
description: '現在のテナントで所有しているすべてのアプリによって作成された schemaextension オブジェクトの一覧を取得します ( '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a320cc0261c40ee8b87dcc658c6ca146d77190e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537777"
---
# <a name="list-schemaextensions"></a>schemaExtensions を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

現在のテナントで所有しているすべてのアプリによって作成された[schemaextension](../resources/schemaextension.md)オブジェクトの一覧を取得します (これは、**開発**中、**使用可能**、または**廃止**され**た場合があります)。また、その他のアプリが所有するすべてのスキーマ拡張機能利用可能**です。 

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
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Content-Type   | application/json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schemaextension](../resources/schemaextension.md)オブジェクトのコレクションを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例は、一意の**id**でフィルター処理することによって、特定のアクセス可能なすべての拡張機能を確認する方法を示しています。 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
