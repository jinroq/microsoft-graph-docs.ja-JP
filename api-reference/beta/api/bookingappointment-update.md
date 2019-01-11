---
title: Bookingappointment を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: baedaf0e894dfdda96c43ff9dc0cb47ce796db9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809682"
---
# <a name="update-bookingappointment"></a>Bookingappointment を更新します。

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
指定された[bookingbusiness](../resources/bookingbusiness.md)で、 [bookingAppointment](../resources/bookingappointment.md)オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All   |
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

| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の SMTP アドレスです。|
|customerId|String|この予定の[bookingCustomer](../resources/bookingcustomer.md)の ID です。 ID が指定されていない場合、予定を作成するとき、新しい**bookingCustomer**オブジェクトが作成されます。 1 回に設定する必要があります **[得意先コード]** 不変です。|
|customerLocation|[location](../resources/location.md)|予定を予約する、 [bookingCustomer](../resources/bookingcustomer.md)の場所の情報を表します。|
|様|String|お客様の名前です。|
|customerNotes|String|この予定に関連付けられている顧客からのノート。 その ID ではこの**bookingAppointment**を表示する場合のみ値を取得することができます。 <br> 最初に顧客との新しい予定を作成する場合にのみ、このプロパティを設定することができます。 その後も、 **[得意先コード]** で表される顧客からの値が計算されます。|
|customerPhone|String|お客様の電話番号です。|
|duration|Duration|[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、予定の長さです。 |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|日付、時刻、およびタイム ゾーンの予定を終了します。|
|invoiceAmount|倍精度浮動小数点数|請求書の請求金額です。|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|日付、時刻、および請求書のこの予定のタイム ゾーンです。|
|invoiceId|String|請求書の ID。|
|invoiceStatus|文字列| 請求書の状態です。 使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft の予約で請求書の URL です。|
|optOutOfCustomerEmail|ブール型|True は、この予定の[bookingCustomer](../resources/bookingcustomer.md)は、この予定の確認メッセージを表示するのには望んでいないことを示します。|
|事後バッファリング|Duration|クリーンアップ、例として、予定が終了した後に予約する時間の量。 値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。 |
|事前バッファリング|Duration|例として、準備のため、予定の開始前に予約する時間の量。 値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。|
|価格|倍精度浮動小数点数|指定された[bookingService](../resources/bookingservice.md)の予定の正規の価格です。|
|priceType|文字列| サービスの価格設定構造の柔軟性を提供するように設定します。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|アラーム|[bookingReminder](../resources/bookingreminder.md)コレクション|この予定に送信される顧客の事前通知のコレクションです。 その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。|
|selfServiceAppointmentId|String|予定が作成された場合 [スケジュール] ページで、お客様が直接にではなく、お客様の代わりにスタッフのメンバーでは、予定の他の追跡 ID。|
|serviceId|String|[BookingService](../resources/bookingservice.md)の ID は、この予定に関連付けられています。|
|serviceLocation|[location](../resources/location.md)|サービスの配信場所です。|
|serviceName|String|**BookingService**の名前は、この予定に関連付けられています。<br>新しい予定を作成するとき、このプロパティは省略可能です。 指定されていない場合は、 **serviceId**プロパティにより、予定に関連付けられたサービスから計算されます。|
|serviceNotes|String|の[bookingStaffMember](../resources/bookingstaffmember.md)からのノート。 その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。|
|staffMemberIds|String コレクション|この予定にスケジュールされている各[bookingStaffMember](../resources/bookingstaffmember.md)の ID です。|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|日付、時刻、およびタイム ゾーンの予定の開始をします。|


## <a name="response"></a>応答
成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。
## <a name="example"></a>例
##### <a name="request"></a>要求
次の例では、サービスが、1 日の日付を変更し、請求書の日付を更新します。
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
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
