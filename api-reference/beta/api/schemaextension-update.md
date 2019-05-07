---
title: schemaExtension を更新する
description: 指定した schemaExtension の定義のプロパティを更新します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: d671f743d1e10c80d713e8efba4e917d3dbd31dd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638922"
---
# <a name="update-schemaextension"></a>schemaExtension を更新する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[Schemaextension](../resources/schemaextension.md)の定義のプロパティを更新します。

この更新は、拡張機能の**Targettypes**プロパティに含まれるすべてのリソースに適用されます。 これらのリソースは、[サポート](/graph/extensibility-overview#supported-resources)されているリソースの種類の中にあります。

拡張機能が**Indevelopment**または**Available** status にある場合は、スキーマ拡張機能 (所有者アプリ) を作成したアプリのみが拡張機能を追加で更新できます。 つまり、アプリでカスタムプロパティを削除したり、ターゲットリソースの種類を定義から削除したりすることはできません。 ただし、アプリで拡張機能の説明を変更することはできます。

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
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Content-Type   | application/json |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|description|String|スキーマ拡張機能の説明。|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション|スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。 加法変更のみが許可されます。 |
|status|String|スキーマ拡張機能のライフサイクル状態。 作成時の初期状態は**開発**中です。 可能な状態遷移は**開発**から**利用可能**であり、**廃止**から利用**可能**です。|
|targetTypes|String コレクション|スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。  加法変更のみが許可されます。|

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a>応答

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/update_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_schemaextension-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>関連項目

- [拡張機能を使用したリソースへのカスタム データの追加](/graph/extensibility-overview)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
