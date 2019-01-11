---
title: 'TableRowCollection: add　'
description: 'テーブルの末尾に行を追加します。 API がこの API を使用して複数の行データを受け入れることができることに注意してください。 一度に 1 行を追加すると、パフォーマンスが低下する可能性があります。 推奨されるアプローチは、1 つの行の挿入を行うのではなく、1 回の呼び出しでまとめて行をバッチ処理することです。 最良の結果を得るには、収集アプリケーション側で挿入して、1 つの行を実行する行操作を追加します。 理想的な 1 つの API 呼び出しで使用する行の数を決定する行の番号を試してください。 '
localization_priority: Normal
ms.openlocfilehash: 131f574186a1c9813a6c9fb8ab6bd4a068da0b3d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870925"
---
# <a name="tablerowcollection-add"></a>TableRowCollection: add　

テーブルの末尾に行を追加します。 API がこの API を使用して複数の行データを受け入れることができることに注意してください。 一度に 1 行を追加すると、パフォーマンスが低下する可能性があります。 推奨されるアプローチは、1 つの行の挿入を行うのではなく、1 回の呼び出しでまとめて行をバッチ処理することです。 最良の結果を得るには、収集アプリケーション側で挿入して、1 つの行を実行する行操作を追加します。 理想的な 1 つの API 呼び出しで使用する行の数を決定する行の番号を試してください。 

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

| パラメーター    | Type   |説明|
|:---------------|:--------|:----------|
|index|Int32|省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。|
|values|Json|省略可能。テーブルの行の書式設定されていない値の 2 次元の配列。|

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[WorkbookTableRow](../resources/tablerow.md)オブジェクトです。

## <a name="example"></a>例
この例では、テーブルの末尾に 2 行のデータが挿入されます。 

##### <a name="request"></a>要求
以下は、要求の例です。
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
