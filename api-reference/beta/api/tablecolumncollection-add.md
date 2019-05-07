---
title: 'TableColumnCollection: 追加'
description: テーブルに新しい列を追加します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3cd267b13b416c3a32b3d2d95eb47c601349e2ee
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637725"
---
# <a name="tablecolumncollection-add"></a>TableColumnCollection: 追加

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テーブルに新しい列を追加します。
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
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

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
|index|number|新しい列の相対位置を指定します。この位置の前の列は右にシフトされます。インデックス値は、最後の列のインデックス値と等しいか、小さくなります。そのため、テーブルの末尾に列を追加するためには使用できません。0 を起点とする番号になります。|
|values|(boolean または string または number) コレクション|省略可能。テーブルの列の、書式設定されていない値の 2 次元の配列。|

## <a name="response"></a>応答

成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[workbookTableColumn](../resources/workbooktablecolumn.md)オブジェクトを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
