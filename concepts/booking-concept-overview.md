---
title: Microsoft Bookings API の概要 (プレビュー)
description: Microsoft Bookings は、小規模企業およびその顧客を対象とした、シンプルかつ効率的な予約スケジュールのためのオンラインおよびモバイルのアプリを提供します。 自動車修理工場、美容院、法律事務所など、予約を扱うサービスを提供する小規模企業で予約管理機能を活用すれば、それによって空いた時間を、事業拡大に向けたより重要な作業に当てることができます。 Microsoft Bookings は、Office 365 Business Premium サブスクリプションを取得した企業がご利用いただけます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: bookings
scenarios: getting-started
ms.openlocfilehash: 83322a2b1343e71f43cd8196ed7484e463ec6ecd
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792948"
---
# <a name="microsoft-bookings-api-overview-preview"></a>Microsoft Bookings API の概要 (プレビュー)

Microsoft Bookings は、小規模企業およびその顧客を対象とした、シンプルかつ効率的な予約スケジュールのためのオンラインおよびモバイルのアプリを提供します。 自動車修理工場、美容院、法律事務所など、予約を扱うサービスを提供する小規模企業で予約管理機能を活用すれば、それによって空いた時間を、事業拡大に向けたより重要な作業に当てることができます。 Microsoft Bookings は、Office 365 Business Premium サブスクリプションを取得した企業がご利用いただけます。

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Microsoft Graph を利用して Microsoft Bookings を統合する理由

### <a name="streamline-appointment-booking"></a>予約管理を合理化する
業務担当者が、かかってきた電話に応対できなかった場合や営業時間外の場合でも、顧客が予約を入れるチャンスを逃すことがありません。 顧客は、事業者の Web サイトや Facebook の予定確認ページでいつでも[利用可能なサービス](/graph/api/bookingbusiness-list-services?view=graph-rest-beta)や[予約状況](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta)を確認できます。 

業務担当者は、どこにいても Web、モバイル アプリ、対面、電話により予約を受け付けることができます。 既存の予約の[変更](/graph/api/bookingappointment-update?view=graph-rest-beta)、[キャンセル](/graph/api/bookingappointment-cancel?view=graph-rest-beta)、または別のスタッフ メンバーへの[再割り当て](/graph/api/bookingappointment-update?view=graph-rest-beta)を実行できます。 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>予約不履行が少なくなり、スタッフの生産性が向上する
事業担当者は予約やキャンセルに関する最低限の通知を含む[スケジュール ポリシー](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta)を指定することができます。一方、顧客は、予約を入れたり変更したりする作業を自分で実行できます。 顧客からの予約確認や事業者側からの予約確認が自動化されるため、予約不履行が少なくなり、スタッフは自分の勤務時間をより有効に利用することができます。 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>どんな場所にいても顧客情報や顧客との関係を管理できる
顧客がすでに[顧客リスト](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta)に記載されているなら、予約履行のための確認が自動的になされます。また必要なら顧客の名前とメール アドレスがリストに[追加](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta)されます。 これは、業務担当者が顧客との接触を保ち、定期的にお知らせや販売促進資料を送付する上で便利です。

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Microsoft Graph での生産性向上およびチーム コラボレーション サービスの統合
同じ Microsoft Graph REST 統一エンドポイントを使用することにより、Bookings API にアクセスし、[Microsoft 365 の優れた機能を統合](overview-major-services.md)することにより、豊富なシナリオをサポートすることができます。 たとえば [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) を使用して事業の財務データを追跡および分析し、本格的なレポートを生成したり、[SharePoint](sharepoint-concept-overview.md) や [Microsoft Teams](teams-concept-overview.md) を使用してチーム コラボレーションを推進したりできます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

「[Microsoft Graph ベータ版の Microsoft Bookings API](/graph/api/resources/booking-api-overview?view=graph-rest-beta)」を参照してください。


## <a name="next-steps"></a>次のステップ

次の詳細情報をご確認ください:

- [Microsoft Bookings](https://support.office.com/ja-JP/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) およびその他の [Office 365 ビジネス アプリ](https://support.office.com/ja-JP/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US)。
- Microsoft Graph における [Bookings API の利用](/graph/api/resources/booking-api-overview?view=graph-rest-beta)。

