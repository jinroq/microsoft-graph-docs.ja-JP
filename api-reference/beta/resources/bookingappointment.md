---
title: bookingAppointment リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0314c8a4d451625c2ee1df332c342c1871a098ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934094"
---
# <a name="bookingappointment-resource-type"></a>bookingAppointment リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
[BookingService](bookingservice.md)Microsoft の予約ビジネスによって提供される、スタッフ メンバーのセットによって実行されるため、顧客の予定を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リストの予定](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md)コレクション | 指定された[bookingbusiness](../resources/bookingbusiness.md)では、 **bookingAppointment**オブジェクトのリストを取得します。 |
|[BookingAppointment を作成します。](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | 指定した[bookingbusiness](../resources/bookingbusiness.md)用の新しい**bookingAppointment**を作成します。 |
|[BookingAppointment を取得します。](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |プロパティと**bookingAppointment**オブジェクトの関係を参照してください。|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |**BookingAppointment**オブジェクトを更新します。 |
|[Delete](../api/bookingappointment-delete.md) | なし |**BookingAppointment**オブジェクトを削除します。 |
|[Cancel](../api/bookingappointment-cancel.md)|なし| **BookingAppointment**オブジェクトをキャンセルします。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|customerEmailAddress|String|予定を予約する、 [bookingCustomer](bookingcustomer.md)の SMTP アドレスです。|
|customerId|String|この予定の[bookingCustomer](bookingcustomer.md)の ID です。 ID が指定されていない場合、予定を作成するとき、新しい**bookingCustomer**オブジェクトが作成されます。 1 回に設定する必要があります **[得意先コード]** 不変です。|
|customerLocation|[location](location.md)|予定を予約する、 [bookingCustomer](bookingcustomer.md)の場所の情報を表します。|
|様|String|お客様の名前です。|
|customerNotes|String|この予定に関連付けられている顧客からのノート。 その ID ではこの**bookingAppointment**を表示する場合のみ値を取得することができます。 <br> 最初に顧客との新しい予定を作成する場合にのみ、このプロパティを設定することができます。 その後も、 **[得意先コード]** で表される顧客からの値が計算されます。|
|customerPhone|String|お客様の電話番号です。|
|duration|Duration|[ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表される、予定の長さです。 |
|end|[dateTimeTimeZone](datetimetimezone.md)|日付、時刻、およびタイム ゾーンの予定を終了します。|
|id|String| **BookingAppointment**の ID です。 読み取り専用です。|
|invoiceAmount|倍精度浮動小数点数|請求書の請求金額です。|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|日付、時刻、および請求書のこの予定のタイム ゾーンです。|
|invoiceId|String|請求書の ID。|
|invoiceStatus|文字列| 請求書の状態です。 使用可能な値: `draft`、`reviewing`、`open`、`canceled`、`paid`、`corrective`。|
|invoiceUrl|String|Microsoft の予約で請求書の URL です。|
|optOutOfCustomerEmail|ブール型|True は、この予定の[bookingCustomer](bookingcustomer.md)は、この予定の確認メッセージを表示するのには望んでいないことを示します。|
|事後バッファリング|Duration|クリーンアップ、例として、予定が終了した後に予約する時間の量。 値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。 |
|事前バッファリング|Duration|例として、準備のため、予定の開始前に予約する時間の量。 値は、 [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html)形式で表されます。|
|価格|倍精度浮動小数点数|指定された[bookingService](bookingservice.md)の予定の正規の価格です。|
|priceType|文字列| サービスの価格設定構造の柔軟性を提供するように設定します。 可能な値は、`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet` です。|
|アラーム|[bookingReminder](bookingreminder.md)コレクション|この予定に送信される顧客の事前通知のコレクションです。 その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。|
|selfServiceAppointmentId|String|予定が作成された場合 [スケジュール] ページで、お客様が直接にではなく、お客様の代わりにスタッフのメンバーでは、予定の他の追跡 ID。|
|serviceId|String|[BookingService](bookingservice.md)の ID は、この予定に関連付けられています。|
|serviceLocation|[location](location.md)|サービスの配信場所です。|
|serviceName|String|**BookingService**の名前は、この予定に関連付けられています。<br>新しい予定を作成するとき、このプロパティは省略可能です。 指定されていない場合は、 **serviceId**プロパティにより、予定に関連付けられたサービスから計算されます。|
|serviceNotes|String|の[bookingStaffMember](bookingstaffmember.md)からのノート。 その ID ではこの**bookingAppointment**を読み取るときにのみ、このプロパティの値があります。|
|staffMemberIds|String コレクション|この予定にスケジュールされている各[bookingStaffMember](bookingstaffmember.md)の ID です。|
|start|[dateTimeTimeZone](datetimetimezone.md)|日付、時刻、およびタイム ゾーンの予定の開始をします。|

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
