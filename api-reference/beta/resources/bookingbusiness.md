---
title: bookingbusiness リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 12b075d273e0228466db063b2c9b91232c32fc2c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328256"
---
# <a name="bookingbusiness-resource-type"></a>bookingbusiness リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Microsoft 予約のビジネスを表します。 これは、Microsoft の予約 API の最上位レベルのオブジェクトです。 これには、ビジネス情報と、予定、顧客、サービス、スタッフメンバーなどの関連するビジネスオブジェクトが含まれています。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[bookingbusinesses のリスト](../api/bookingbusiness-list.md) | [bookingbusiness](bookingbusiness.md)コレクション |テナント内の bookingbusiness オブジェクトのコレクションを取得します。 |
|[bookingbusiness の作成](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | 新しい Microsoft 予約ビジネスを作成します。 |
|[bookingbusiness の取得](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |bookingbusiness オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |**bookingbusiness**オブジェクトのプロパティを更新します。 |
|[Delete](../api/bookingbusiness-delete.md) | なし |**bookingbusiness**オブジェクトを削除します。 |
|[bookingappointment の作成](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| 予定のコレクションに投稿して、新しいブックを作成します。|
|[予定を一覧表示する](../api/bookingbusiness-list-appointments.md) |[bookingappointment](bookingappointment.md)コレクション| bookingappointment オブジェクトコレクションを取得します。|
|[bookingcustomer の作成](../api/bookingbusiness-post-customers.md) |[bookingcustomer](bookingcustomer.md)| customers コレクションへの投稿により、新しい書店の顧客を作成します。|
|[顧客を一覧表示する](../api/bookingbusiness-list-customers.md) |[bookingcustomer](bookingcustomer.md)コレクション| bookingcustomer オブジェクトのコレクションを取得します。|
|[bookingservice の作成](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| サービスコレクションへの投稿により、新しい bookingservice を作成します。|
|[サービスを一覧表示する](../api/bookingbusiness-list-services.md) |[bookingservice](bookingservice.md)コレクション| bookingservice オブジェクトのコレクションを取得します。|
|[bookingStaffMember を作成する](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| staffMembers コレクションへの投稿によって新しい bookingStaffMember を作成します。|
|[リスト staffMembers](../api/bookingbusiness-list-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)コレクション| bookingStaffMember オブジェクトのコレクションを取得します。|
|[List calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingappointment](bookingappointment.md)コレクション|指定した日付範囲内に発生する**bookingappointment**オブジェクトのコレクションを取得します。|
|[publish](../api/bookingbusiness-publish.md)|なし|この業務の [スケジュール] ページを外部のお客様が利用できるようにします。 **isPublished**プロパティを true に、 **publicurl**プロパティを [スケジュール] ページの URL に設定します。|
|[unpublish](../api/bookingbusiness-unpublish.md)|なし| 外部のお客様がこの業務のスケジュール設定ページを使用できないようにします。 **isPublished**プロパティを false に設定し、 **publicurl**プロパティを null に設定します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|会社の住所。 **住所**プロパティは、 **phone**および**webSiteUrl**と共に、ビジネススケジュールページのフッターに表示されます。|
|microsoft.rtc.rgs.management.writablesettings.businesshours|[bookingwork hours](bookingworkhours.md)コレクション|業務の運営時間。|
|businessType|String|業務の種類。|
|defaultCurrencyIso|String|Microsoft の予約で勤務している通貨のコード。|
|displayName|String|顧客とのインターフェイスとなるビジネスの名前。 この名前は、[ビジネススケジュール] ページの上部に表示されます。|
|email|String|ビジネスの電子メールアドレス。|
|id|String|ビジネスの一意なプログラム id。 読み取り専用です。|
|isPublished|Boolean|[スケジュール] ページは、外部のお客様が利用できるようになっています。 **発行**および**未発行**アクションを使用して、このプロパティを設定します。 読み取り専用です。|
|phone|String|会社の電話番号。 [**電話**] プロパティは、[**住所**] および [ **webSiteUrl**] と共に、[ビジネススケジュール] ページのフッターに表示されます。|
|publicurl|String|ページの公開または[発行](../api/bookingbusiness-publish.md)を[取り消し](../api/bookingbusiness-unpublish.md)た後に設定される、[スケジュール] ページの URL。 読み取り専用です。|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|このビジネスに対して予約を作成する方法を指定します。|
|webSiteUrl|String|ビジネス web サイトの URL。 **webSiteUrl**プロパティは、[**住所**, **phone**] と共に、[ビジネススケジュール] ページのフッターに表示されます。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|予定|[bookingappointment](bookingappointment.md)コレクション| このビジネスのすべての予定。 読み取り専用です。 Null 許容型。|
|calendarView|[bookingappointment](bookingappointment.md)コレクション| 指定した日付範囲内の、このビジネスの一連の予定。 読み取り専用です。 Null 許容型。|
|ユーザー|[bookingcustomer](bookingcustomer.md)コレクション| このビジネスのすべてのお客様。 読み取り専用です。 Null 許容型。|
|サービス|[bookingservice](bookingservice.md)コレクション| このビジネスによって提供されるすべてのサービス。 読み取り専用です。 Null 許容型。|
|staffMembers|[bookingStaffMember](bookingstaffmember.md)コレクション| このビジネスのサービスを提供するすべてのスタッフメンバー。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
