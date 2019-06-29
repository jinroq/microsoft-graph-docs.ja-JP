---
title: schemaExtension の作成
description: サポートするリソースの種類を拡張するために、schemaExtension 定義を新規作成します。
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: b717215b6361d0523bfb485208a2a6b3756f987d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277330"
---
# <a name="create-schemaextension"></a>schemaExtension の作成

[サポートするリソースの種類](/graph/extensibility-overview#supported-resources)を拡張するために、[schemaExtension](../resources/schemaextension.md) 定義を新規作成します。

スキーマ拡張機能により、厳密に型指定されたカスタム データをリソースに追加することができます。スキーマ拡張機能を作成するアプリは、所有者アプリです。拡張機能の[状態](/graph/extensibility-overview#schema-extensions-lifecycle)によっては、拡張機能を更新または削除できるのは、所有者アプリだけです。 

[トレーニング コースを説明するスキーマ拡張機能を定義する](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course)方法、スキーマ拡張定義を使用して[トレーニング コース データで新規グループを作成する](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data)方法、[既存グループにトレーニング コース データを追加する](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group)方法については、それぞれの例を参照してください。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。

次の表に、スキーマ拡張機能の作成時に必要なプロパティを示します。

| パラメーター | 型 | 説明|
|:---------------|:--------|:----------|
|description|String|スキーマ拡張機能の説明。|
|id|String|スキーマ拡張機能の定義の一意の識別子。 <br>値の割り当ては、以下の 2 方法のいずれかで行うことができます。 <ul><li>確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。 次に例 `contoso_mySchema` を示します。 注: 上位ドメイン `.com`、`.net`、`.gov`、`.edu`、`.org` の下では、検証済みのドメインのみがサポートされます。 </li><li>スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</li></ul>作成後、このプロパティは変更できません。 |
|owner|String|(省略可能) スキーマ拡張機能の所有者であるアプリケーションの `appId` です。 このプロパティは作成時に指定して所有者を設定できます。  指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。 たとえば、Graph エクスプローラーを使用して新しいスキーマ拡張機能の定義を作成する場合は、所有者プロパティを指定する**必要があります**。 設定すると、このプロパティは読み取り専用で、変更することはできません。|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション|スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。|
|targetTypes|String collection|このスキーマ拡張機能の定義を適用できる、(スキーマ拡張機能をサポートしている) 一連の Microsoft Graph のリソースの種類。|

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `201 Created` 応答コードと、[schemaExtension](../resources/schemaextension.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request-1"></a>要求 1

最初の例では、確認済みのドメイン名 `graphlearn` とスキーマ名 `courses` を使用して、スキーマ拡張機能の定義の **id** プロパティの一意の文字列を形成します。一意の文字列は次の形式に基づきます。\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。

要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-1"></a>応答 1

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a>要求 2

2 番目の例では、要求の **id** プロパティ内のスキーマ名 `courses` だけを指定し、[schemaExtension](../resources/schemaextension.md) オブジェクト内の残りのプロパティを JSON 表記で指定しています。Microsoft Graph は一意の文字列値を割り当て、それを応答内で返します。

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-2"></a>応答 2

応答には、要求の中で提供されているスキーマ名に基づいた一意の文字列がその **id** プロパティ内に含まれ、新規作成したスキーマ定義の残りの部分も応答に含まれています。応答の中の **id** の値は、次の形式に基づきます。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_2-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_schemaextension_from_schemaextensions_2-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a>関連項目

- [拡張機能を使用したリソースへのカスタム データの追加](/graph/extensibility-overview)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/schemaextension-post-schemaextensions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/schemaextension-post-schemaextensions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/schemaextension-post-schemaextensions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/schemaextension-post-schemaextensions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/schemaextension-post-schemaextensions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
