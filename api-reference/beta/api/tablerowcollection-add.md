---
title: 'TableRowCollection: add　'
description: '表の末尾に行を追加します。 この api を使用して複数行データを受け入れることができることに注意してください。 一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。 推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。 最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。 行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fbc4d8d3b0f5a1653bf4d022dfea8c68c5401d18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544558"
---
# <a name="tablerowcollection-add"></a>TableRowCollection: add　

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表の末尾に行を追加します。 この api を使用して複数行データを受け入れることができることに注意してください。 一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。 推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。 最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。 行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。 

## <a name="error-handling"></a>エラー処理

この要求に対して、504 HTTP エラーが表示されることがあります。 このエラーに対する適切な対応は、要求を繰り返すことです。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite    |
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
|index|number|省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。|
|values|(boolean、string、または number)|省略可能。 表の行の書式設定されていない値の2次元配列。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。

## <a name="example"></a>例
この例では、テーブルの最後に2行のデータが挿入されます。 

##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
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
  "@odata.type": "microsoft.graph.tableRow"
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablerowcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
