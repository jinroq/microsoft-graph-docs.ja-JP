---
title: 'workbookApplication: 計算'
description: Excel で現在開いているすべてのブックを再計算します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2e3a980ae7eab1dd3032ae68b180019ae4c7ceee
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636976"
---
# <a name="workbookapplication-calculate"></a>workbookApplication: 計算

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excel で現在開いているすべてのブックを再計算します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|calculationType|string|使用する計算の種類を指定します。  可能な値は、`Recalculate`、`Full`、`FullRebuild` です。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
