---
title: 範囲:BoundingRect
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 54a8fea095909d199f2cd2b74e2512f6c2f05a6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876616"
---
# <a name="range-boundingrect"></a>範囲:BoundingRect

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

指定した範囲を包含する、最小の Range オブジェクトを取得します。たとえば、"B2:C5" と "D10:E15" の GetBoundingRect は、"B2:E16" になります。
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
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

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
|anotherRange|文字列|Range オブジェクト、アドレスまたは範囲名。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。

## <a name="example"></a>例
以下は、この API を呼び出す方法の例です。
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
