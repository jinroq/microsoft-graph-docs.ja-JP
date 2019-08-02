---
title: Microsoft Graph で Microsoft Bookings API を使用する
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: 171f75d35812176202263659185bd4dca94e06de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974200"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Microsoft Graph で Microsoft Bookings API を使用する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Microsoft Bookings では、中小企業のオーナーが最小限の設定で顧客の予約と情報を管理できます。 ビジネス オーナーは、一連のサービスを提供するビジネスを 1 つ以上作成できます。 オーナーはスタッフを設定し、各スタッフが実施するサービスを指定できます。 顧客は当該ビジネスの特定のサービスをオンラインまたはモバイル アプリから予約できます。 Bookings では、ビジネス、スタッフ、顧客に対し常に最新の予約情報が提供されます。

Bookings API の [bookingBusiness](bookingbusiness.md) は、プログラムで次のオブジェクトを使用します。
 
- 1 つまたは複数の [bookingStaffMember](bookingstaffmember.md) オブジェクト
- 1 つまたは複数の [bookingService](bookingservice.md) オブジェクト
- 一連の[bookingAppointment](bookingappointment.md)インスタンス
- 一連の[bookingCustomer](bookingcustomer.md)オブジェクト

## <a name="using-the-bookings-rest-api"></a>Bookings REST API を使用する

顧客の予約を初めて受け付ける前に、次の手順を行います。 対応する操作のための適切な[アクセス トークン](/graph/auth-overview)を提供していることを確認します。

1. ビジネスで [Office 365 Business Premium](https://products.office.com/ja-JP/business/office-365-business-premium) サブスクリプションを購入していることを確認します。
2. エンティティ セットに POST 操作を送信して新しい **bookingBusiness** を作成します。 最小限でも、顧客に対して表示される新しいビジネスの名前を指定してください。
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
POST 応答で返される新しい **bookingBusiness** の **id** プロパティを使用して、ビジネス設定を[カスタマイズ](../api/bookingbusiness-update.md)し、ビジネスのスタッフとサービスを追加します。

3. ビジネスの個々のスタッフを追加します。
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. ビジネスで提供する各サービスを定義します。
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. ビジネスのスケジュール ページを公開し、顧客とビジネス運営担当者が予約の受付を開始できるようにします。
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

一般に、Office 365 テナントの予約ビジネスをすべて一覧表示するには次のようにします。
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>一般的なユース ケース 

次の表は、Bookings API でのビジネスの一般的な操作を示します。

| ユース ケース        | REST リソース | 関連項目 |
|:---------------|:--------|:----------|
| ビジネスの作成、取得、更新、または削除 | [bookingBusiness](bookingbusiness.md) | [bookingBusiness のメソッド](bookingbusiness.md#methods) |
| スケジュール ポリシーの更新 | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [bookingBusiness を更新する](../api/bookingbusiness-update.md) |
| スタッフの追加、取得、更新、または削除 | [bookingStaffMember](bookingstaffmember.md) | [bookingStaffMember のメソッド](bookingstaffmember.md#methods)  |
| サービスの追加、取得、更新、または削除 | [bookingService](bookingservice.md) | [bookingService のメソッド](bookingservice.md#methods)  |
| スケジュール ページの公開または公開の取り消し | [bookingBusiness](bookingbusiness.md) | [publish](../api/bookingbusiness-publish.md) <br> [unpublish](../api/bookingbusiness-unpublish.md) |
| 予約の作成、取得、更新、削除、またはキャンセル | [bookingAppointment](bookingappointment.md) | [bookingAppointment のメソッド](bookingappointment.md#methods)  |
| 日付範囲内の予約の取得 | [bookingBusiness](bookingbusiness.md) | [List Bookings calendarView](../api/bookingbusiness-list-calendarview.md) |
| 通貨の取得 | [bookingCurrency](bookingcurrency.md) | [bookingCurrency のメソッド](bookingcurrency.md#methods) |


## <a name="see-also"></a>関連項目

- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。
- 「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。
- Microsoft Graph で[権限](/graph/permissions-reference)を選択する方法を理解してください。
