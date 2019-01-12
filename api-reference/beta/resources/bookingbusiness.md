---
title: bookingBusiness リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cf00239802cec9a705c24548649e38f3022383a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986216"
---
# <a name="bookingbusiness-resource-type"></a>bookingBusiness リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
Microsoft 予約でビジネスを表します。 これは、Microsoft 予約 API 内の最上位オブジェクトです。 ビジネス情報や予定、顧客、サービス、スタッフなどの関連するビジネス オブジェクトが含まれています。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト bookingBusinesses](../api/bookingbusiness-list.md) | [bookingBusiness](bookingbusiness.md)コレクション |テナント内には、bookingbusiness オブジェクトのコレクションを取得します。 |
|[BookingBusiness を作成します。](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 新しい Microsoft 予約ビジネスを作成します。 |
|[BookingBusiness を取得します。](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |BookingBusiness オブジェクトのプロパティと関係を参照してください。|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |**BookingBusiness**オブジェクトのプロパティを更新します。 |
|[Delete](../api/bookingbusiness-delete.md) | なし |**BookingBusiness**オブジェクトを削除します。 |
|[BookingAppointment を作成します。](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 予定のコレクションへの投稿には、新しい bookingAppointment を作成します。|
|[リストの予定](../api/bookingbusiness-list-appointments.md) |[bookingAppointment](bookingappointment.md)コレクション| BookingAppointment オブジェクトのコレクションを取得します。|
|[BookingCustomer を作成します。](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| お客様のコレクションへの投稿には、新しい bookingCustomer を作成します。|
|[顧客のリスト](../api/bookingbusiness-list-customers.md) |[bookingCustomer](bookingcustomer.md)コレクション| BookingCustomer オブジェクトのコレクションを取得します。|
|[BookingService を作成します。](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| サービスのコレクションへの投稿には、新しい bookingService を作成します。|
|[サービスの一覧](../api/bookingbusiness-list-services.md) |[bookingService](bookingservice.md)コレクション| BookingService オブジェクトのコレクションを取得します。|
|[BookingStaffMember を作成します。](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| StaffMembers コレクションへの投稿には、新しい bookingStaffMember を作成します。|
|[リスト staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)コレクション| BookingStaffMember オブジェクトのコレクションを取得します。|
|[calendarView を一覧表示する](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](bookingappointment.md)コレクション|指定した日付範囲内に発生する**bookingAppointment**オブジェクトのコレクションを取得します。|
|[発行](../api/bookingbusiness-publish.md)|なし|このビジネスのスケジュール ページを外部の顧客が使用できるようにします。 True の場合、およびスケジュールのページの URL を**publicUrl**プロパティに**isPublished**プロパティを設定します。|
|[公開取り下げ](../api/bookingbusiness-unpublish.md)|なし| 外部の顧客に、利用できないこのビジネスでのスケジュールのページを加えます。 **IsPublished**プロパティを false、および**publicUrl**プロパティを null に設定します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|ビジネスの住所。 **電話**と**webSiteUrl**と、**アドレス**のプロパティは、ビジネスのスケジュール ページのフッターに表示されます。|
|businessHours|[bookingWorkHours](bookingworkhours.md)コレクション|ビジネスの操作の時間です。|
|businessType|String|ビジネスの種類。|
|defaultCurrencyIso|String|ビジネスが Microsoft 予約上で動作する通貨コード。|
|displayName|String|ビジネスでは、お客様とのインターフェイスの名前。 ページをスケジューリングするビジネスの先頭にこの名前が表示されます。|
|email|String|ビジネスの電子メール アドレスです。|
|id|String|ビジネス用の一意なプログラム識別子です。 読み取り専用です。|
|isPublished|ブール型|スケジュール ページが可能となって外部の顧客にします。 このプロパティを設定するのにには、**公開**し、**非公開**のアクションを使用します。 読み取り専用です。|
|phone|String|ビジネスの電話番号です。 **電話**は、**アドレス**と**webSiteUrl**とは、ビジネスのスケジュール ページのフッターに表示されます。|
|publicUrl|String|ページ[を公開](../api/bookingbusiness-publish.md)するか[非公開](../api/bookingbusiness-unpublish.md)に設定されているスケジュールのページの URL です。 読み取り専用です。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|このビジネスでの予約を作成する方法を指定します。|
|webSiteUrl|String|ビジネスの web サイトの URL です。 **アドレス**、**電話**、および、 **webSiteUrl**プロパティは、ビジネスのスケジュール] ページのフッターに表示されます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|appointments|[bookingAppointment](bookingappointment.md)コレクション| このビジネスのすべての予定です。 読み取り専用です。 Null 許容型。|
|calendarView|[bookingAppointment](bookingappointment.md)コレクション| このビジネスでは、指定した日付範囲内の予定のセット。 読み取り専用です。 Null 許容型。|
|お客様|[bookingCustomer](bookingcustomer.md)コレクション| このビジネスのすべての顧客。 読み取り専用です。 Null 許容型。|
|サービス|[bookingService](bookingservice.md)コレクション| このような企業で提供されているすべてのサービス。 読み取り専用です。 Null 許容型。|
|staffMembers|[bookingStaffMember](bookingstaffmember.md)コレクション| すべてのスタッフはこのような企業にサービスを提供します。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingBusiness"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "businessType": "String",
  "defaultCurrencyIso": "String",
  "displayName": "String",
  "email": "String",
  "id": "String (identifier)",
  "isPublished": true,
  "phone": "String",
  "publicUrl": "String",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "webSiteUrl": "String"
}

```

## <a name="see-also"></a>関連項目


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
