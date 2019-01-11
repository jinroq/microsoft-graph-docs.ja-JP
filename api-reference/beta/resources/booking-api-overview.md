---
title: Microsoft Graph では、Microsoft 予約 API を使用します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845536"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Microsoft Graph では、Microsoft 予約 API を使用します。

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。
 
Microsoft の予約には、スモール ビジネスの経営者がお客様の予約と最小限の設定で情報を管理することができます。 ビジネス所有者は、各業務の一連のサービスを提供することで、1 つまたは複数の企業を作成できます。 所有者では、スタッフのメンバーを設定でき、各スタッフ メンバーを実行するサービスを指定することができます。 顧客は、オンラインまたはモバイル アプリケーションでは、そのビジネスで特定のサービスの予定を予約することができます。 予約する予定の時刻は最新ビジネス、スタッフ、および顧客の関係を保証します。

プログラムを使用して、予約 API では、 [bookingBusiness](bookingbusiness.md)には、次のオブジェクトが含まれます。
 
- 1 つまたは複数の[bookingStaffMember](bookingstaffmember.md)オブジェクト
- 1 つまたは複数の[bookingService](bookingservice.md)オブジェクト
- [BookingAppointment](bookingappointment.md)のインスタンスのセット
- 一連の[bookingCustomer](bookingcustomer.md)オブジェクト

## <a name="using-the-bookings-rest-api"></a>予約 REST API を使用します。

最初にビジネスのお客様の予定を予約する前に、次の手順を説明します。 対応する操作に対して適切な[アクセス トークン](/graph/auth-overview)を提供することを確認します。

1. ビジネスには、 [Office 365 のビジネス プレミアム](https://products.office.com/en-us/business/office-365-business-premium)サブスクリプションを確認します。
2. 新しい**bookingBusiness**を作成するには、POST 操作のエンティティ セットに送信します。 最低限、顧客に表示される新しいビジネスの名前を指定する必要があります。<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
POST 応答で返される新しい**bookingBusiness**の**id**プロパティを使用して、ビジネスの設定の[カスタマイズ](../api/bookingbusiness-update.md)を続行して、スタッフとのビジネスのサービスを追加します。

3. ビジネスの個々 のスタッフのメンバーを追加します。<!-- { "blockType": "ignored" } -->
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
4. ビジネスによって提供される各サービスを定義します。<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. 顧客およびビジネス オペレーターが予約を開始できるようにするのには、ビジネスのスケジュールのページを公開するには。<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

一般で、Office 365 テナント内のすべての予約会社を一覧表示します。<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>一般的なユース ケース 

予約 API でのビジネスの一般的な操作を次の表に一覧します。

| ユース ケース        | REST リソース | 関連項目 |
|:---------------|:--------|:----------|
| ビジネスの作成、取得、更新、削除 | [bookingBusiness](bookingbusiness.md) | [BookingBusiness の方法](bookingbusiness.md#methods) |
| スケジュー リング ポリシーを更新します。 | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [BookingBusiness を更新します。](../api/bookingbusiness-update.md) |
| 追加、取得、更新、またはスタッフのメンバーを削除します。 | [bookingStaffMember](bookingstaffmember.md) | [BookingStaffMember の方法](bookingstaffmember.md#methods)  |
| 追加、取得、更新、またはサービスを削除します。 | [bookingService](bookingservice.md) | [BookingService の方法](bookingservice.md#methods)  |
| 公開または公開取り下げのスケジュール ページ | [bookingBusiness](bookingbusiness.md) | [発行](../api/bookingbusiness-publish.md) <br> [公開取り下げ](../api/bookingbusiness-unpublish.md) |
| 作成、取得、更新、削除、または予定をキャンセル | [bookingAppointment](bookingappointment.md) | [BookingAppointment の方法](bookingappointment.md#methods)  |
| 日付の範囲で予定を取得します。 | [bookingBusiness](bookingbusiness.md) | [予約予定表ビューを一覧表示します。](../api/bookingbusiness-list-calendarview.md) |
| 通貨を取得します。 | [bookingCurrency](bookingcurrency.md) | [BookingCurrency の方法](bookingcurrency.md#methods) |


## <a name="see-also"></a>関連項目

- 
  [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。
- [Microsoft Graph を使ってパートナーのいくつかの方法](https://developer.microsoft.com/graph/graph/examples#partners)を参照してください。
- Graph で[のアクセス許可](/graph/permissions-reference)を選択する方法について説明します。
