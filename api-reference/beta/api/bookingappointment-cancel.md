---
title: 'bookingAppointment: キャンセル'
description: 指定した bookingappointment で指定された bookingAppointment を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c96ed0403e59f4b2dd357514168361fc3bc683f6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636535"
---
# <a name="bookingappointment-cancel"></a>bookingAppointment: キャンセル

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[bookingappointment](../resources/bookingbusiness.md)で指定された[Bookingappointment](../resources/bookingappointment.md)を取り消し、関連する顧客およびスタッフメンバーにメッセージを送信します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  BookingsAppointment すべての予約。すべて、予約....   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。   |
|アプリケーション | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|cancellationMessage|String|予定がキャンセルされたことをお客様に通知するメッセージ。|

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No content` 応答コードを返します。応答本文には何も返されません。

Exisit でない予定を取り消しようとすると、このメソッドはを`HTTP 404 Not found`返します。

## <a name="example"></a>例
この API を呼び出す方法の例を次に示します。
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
