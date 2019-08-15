---
title: Bookingservice を更新する
description: 指定した bookingservice の bookingService オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a9738c22e920635b3ef08dcc97803adb611831c5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419329"
---
# <a name="update-bookingservice"></a>Bookingservice を更新する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[bookingservice](../resources/bookingbusiness.md)の[bookingservice](../resources/bookingservice.md)オブジェクトのプロパティを更新します。

以下に、サービスに対してカスタマイズできる例をいくつか示します。
- Price
- 予定の通常の長さ
- Reminders
- サービスの実行前または完了後にセットアップする任意の時間バッファー
- 予約またはキャンセルするための最小限の通知や、ユーザーが予定に対して特定のスタッフメンバーを選択できるかどうかの[スケジュールポリシー](../resources/bookingschedulingpolicy.md)パラメーター。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  予約します。すべての予約   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。   |
|アプリケーション | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultDuration|期間|サービスの既定の長さ。日数、時間、分、および秒で表されます。 たとえば、P11D23H59M 59.999999999999 S のようになります。 |
|defaultLocation|[location](../resources/location.md)|サービスの既定の物理的な場所。|
|既定の価格|2 行分|サービスの既定の通貨料金。|
|defaultPriceType|string|サービスの既定の課金方法。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|defaultReminders|[Bookingreminder](../resources/bookingreminder.md)コレクション|このサービスの予定に対する既定のアラームのセット。 このプロパティの値は、この**Bookingservice**を ID で読み取る場合にのみ使用できます。|
|description|String|サービスのテキストの説明。|
|displayName|String|サービス名。|
|emailAddress|String|電子メールアドレス|
|id|String| 読み取り専用です。|
|isHiddenFromCustomers|Boolean|True は、このサービスを予約にお客様が利用できないことを意味します。|
|notes|String|このサービスに関する追加情報。|
|postBuffer|期間|このサービスの予定が終了してから、次の顧客の予定が予約されるまでの時間。|
|preBuffer|期間|このサービスの予定を開始できるようになるまでの時間。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|この種類のサービスの予定を作成および管理する方法を決定する一連のポリシー。|
|staffMemberIds|文字列コレクション|このサービスを提供する[スタッフメンバー](../resources/bookingstaffmember.md)を表します。 |

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の使用例は、指定されたサービスの期間を更新します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
