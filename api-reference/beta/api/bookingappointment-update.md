---
title: bookingappointment の更新
description: 指定した bookingappointment の bookingappointment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cca20fa9cca596095f902adf961ea424ff688cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322539"
---
# <a name="update-bookingappointment"></a>bookingappointment の更新

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定した[bookingappointment](../resources/bookingbusiness.md)の[bookingappointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  bookingsappointment すべての予約。すべて、予約....   |
|委任 (個人用 Microsoft アカウント) | サポートされていません。   |
|アプリケーション | サポートされていません。  |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a>オプションの要求ヘッダー
| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|予定を予約している[bookingcustomer](../resources/bookingcustomer.md)の SMTP アドレス。|
|id|String|この予定の[bookingcustomer](../resources/bookingcustomer.md)の ID。 予定の作成時に ID が指定されていない場合は、新しい**bookingcustomer**オブジェクトが作成されます。 設定すると、 **customerId**を不変にすることを考慮する必要があります。|
|顧客の所在地|[location](../resources/location.md)|予定を予約している[bookingcustomer](../resources/bookingcustomer.md)の場所情報を表します。|
|おける|String|顧客の名前を指定します。|
|顧客メモ|String|この予定に関連付けられている顧客からのメモ。 ID でこの**bookingappointment**を読み取る場合にのみ、値を取得できます。 <br> このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。 その時点で、その値は**customerId**で表される顧客から計算されます。|
|顧客電話|String|お客様の電話番号。|
|duration|期間|「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|予定が終了する日付、時刻、タイムゾーン。|
|invoiceAmount|2 行分|請求書の請求金額。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|この予定の請求書の日付、時刻、タイムゾーン。|
|invoiceId|String|請求書の ID。|
|invoiceStatus|string| 請求書の状態。 使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft 予約の請求書の URL。|
|optOutOfCustomerEmail|Boolean|True は、この予定の[bookingcustomer](../resources/bookingcustomer.md)が、この予定の確認を受信したくないことを示します。|
|postbuffer|期間|予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。 この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。 |
|prebuffer|期間|準備のために予定が開始されるまでの時間を例として示します。 この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。|
|代金|2 行分|指定した[bookingservice](../resources/bookingservice.md)の予定に対する正規の価格。|
|priceType|string| サービスの価格構造を柔軟に提供するための設定。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|isp|[bookingreminder](../resources/bookingreminder.md)コレクション|この予定に対して送信された顧客のアラームのコレクションです。 このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。|
|selfServiceAppointmentId|String|顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。|
|serviceId|String|この予定に関連付けられている[bookingservice](../resources/bookingservice.md)の ID です。|
|serviceLocation|[location](../resources/location.md)|サービスが配信される場所。|
|serviceName|String|この予定に関連付けられている**bookingservice**の名前です。<br>新しい予定を作成するときは、このプロパティは省略可能です。 指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。|
|serviceNotes|String|[bookingStaffMember](../resources/bookingstaffmember.md)からのメモ。 このプロパティの値は、この**bookingappointment**を ID で読み取る場合にのみ使用できます。|
|staffMemberIds|String collection|この予定でスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|予定が開始する日付、時刻、タイムゾーン。|


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例では、サービスの日付を日単位に変更し、請求日も更新しました。
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
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
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
