---
title: bookingAppointment リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1956ddac829a2921aba6ebf438ae4815ca56b8d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013130"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Microsoft の予約ビジネスによって提供される、一連のスタッフメンバーによって実行される、 [Bookingservice](bookingservice.md)の顧客の予定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[予定を一覧表示する](../api/bookingbusiness-list-appointments.md) |  [Bookingappointment](bookingappointment.md)コレクション | 指定した[bookingappointment](../resources/bookingbusiness.md)の**bookingappointment**オブジェクトのリストを取得します。 |
|[BookingAppointment の作成](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 指定した[bookingappointment](../resources/bookingbusiness.md)の新しい**ブック**を作成します。 |
|[BookingAppointment を取得する](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |**Bookingappointment**オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |**Bookingappointment**オブジェクトを更新します。 |
|[Delete](../api/bookingappointment-delete.md) | None |**Bookingappointment**オブジェクトを削除します。 |
|[Cancel](../api/bookingappointment-cancel.md)|None| **Bookingappointment**オブジェクトを取り消します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|予定を予約している[Bookingcustomer](bookingcustomer.md)の SMTP アドレス。|
|Id|String|この予定の[Bookingcustomer](bookingcustomer.md)の ID。 予定の作成時に ID が指定されていない場合は、新しい**Bookingcustomer**オブジェクトが作成されます。 設定すると、 **customerId**を不変にすることを考慮する必要があります。|
|顧客の所在地|[location](location.md)|予定を予約している[Bookingcustomer](bookingcustomer.md)の場所情報を表します。|
|おける|String|顧客の名前を指定します。|
|顧客メモ|String|この予定に関連付けられている顧客からのメモ。 ID でこの**Bookingappointment**を読み取る場合にのみ、値を取得できます。 <br> このプロパティは、最初に新しい顧客を使用して予定を作成するときにのみ設定できます。 その時点で、その値は**customerId**で表される顧客から計算されます。|
|顧客電話|String|お客様の電話番号。|
|duration|期間|「文字形式」で示されて[](https://www.iso.org/iso-8601-date-and-time-format.html)いる予定の長さ。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|予定が終了する日付、時刻、タイムゾーン。|
|id|String| **Bookingappointment**の ID。 読み取り専用です。|
|invoiceAmount|2 行分|請求書の請求金額。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|この予定の請求書の日付、時刻、タイムゾーン。|
|invoiceId|String|請求書の ID。|
|invoiceStatus|string| 請求書の状態。 使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft 予約の請求書の URL。|
|optOutOfCustomerEmail|Boolean|True は、この予定の[Bookingcustomer](bookingcustomer.md)が、この予定の確認を受信したくないことを示します。|
|postBuffer|期間|予定が終了した後に、クリーンアップのために確保する時間の長さを例として示します。 この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。 |
|preBuffer|期間|準備のために予定が開始されるまでの時間を例として示します。 この値は、" [](https://www.iso.org/iso-8601-date-and-time-format.html) /" という形式で表されます。|
|代金|2 行分|指定した[Bookingservice](bookingservice.md)の予定に対する正規の価格。|
|priceType|string| サービスの価格構造を柔軟に提供するための設定。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|isp|[Bookingreminder](bookingreminder.md)コレクション|この予定に対して送信された顧客のアラームのコレクションです。 このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。|
|selfServiceAppointmentId|String|顧客に代わってスタッフメンバーではなく、顧客が [スケジュール] ページで直接作成された予定の場合は、予定の追加の追跡 ID。|
|serviceId|String|この予定に関連付けられている[Bookingservice](bookingservice.md)の ID です。|
|serviceLocation|[location](location.md)|サービスが配信される場所。|
|serviceName|String|この予定に関連付けられている**Bookingservice**の名前です。<br>新しい予定を作成するときは、このプロパティは省略可能です。 指定しない場合、 **serviceId**プロパティによって、予定に関連付けられているサービスから計算されます。|
|serviceNotes|String|[BookingStaffMember](bookingstaffmember.md)からのメモ。 このプロパティの値は、この**Bookingappointment**を ID で読み取る場合にのみ使用できます。|
|staffMemberIds|文字列コレクション|この予定でスケジュールされている各[bookingStaffMember](bookingstaffmember.md)の ID。|
|開始|[dateTimeTimeZone](datetimetimezone.md)|予定が開始する日付、時刻、タイムゾーン。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
