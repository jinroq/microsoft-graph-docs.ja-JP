---
title: 'TableRowCollection: add　'
description: '表の末尾に行を追加します。 この api を使用して複数行データを受け入れることができることに注意してください。 一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。 推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。 最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。 行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1cb0a5a05def3028ae8a9309cda5eef7b69ff35a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456058"
---
# <a name="tablerowcollection-add"></a>TableRowCollection: add　

表の末尾に行を追加します。 この api を使用して複数行データを受け入れることができることに注意してください。 一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。 推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。 最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。 行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。 

## <a name="error-handling"></a>エラー処理

この要求に対して、504 HTTP エラーが表示されることがあります。 このエラーに対する適切な対応は、要求を繰り返すことです。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Workbook-Session-Id  | 変更を保持するかどうかを決定するブック セッション ID。省略可能。|

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|index|Int32|省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。|
|values|Json|省略可能。テーブルの行の書式設定されていない値の 2 次元の配列。|

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookTableRow](../resources/tablerow.md)オブジェクトを返します。

## <a name="example"></a>例
この例では、テーブルの最後に2行のデータが挿入されます。 

##### <a name="request"></a>要求
以下は、要求の例です。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
