# <a name="microsoft-bookings-api-overview-preview"></a>Microsoft 予約 API の概要 (プレビュー)

Microsoft Bookings は、小規模企業およびその顧客を対象とした、シンプルかつ効率的な予約スケジュールのためのオンラインおよびモバイルのアプリを提供します。 自動車修理工場、美容院、法律事務所など、予約を扱うサービスを提供する小規模企業で予約管理機能を活用すれば、それによって空いた時間を、事業拡大に向けたより重要な作業に当てることができます。 Microsoft Bookings は、Office 365 Business Premium サブスクリプションを取得した企業がご利用いただけます。

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Microsoft Graph を利用して Microsoft Bookings を統合する理由

### <a name="streamline-appointment-booking"></a>予約管理を合理化する
業務担当者が、かかってきた電話に応対できなかった場合や営業時間外の場合でも、顧客が予約を入れるチャンスを逃すことがありません。 顧客は、事業者の Web サイトや Facebook の予定確認ページでいつでも[利用可能なサービス](../api-reference/beta/api/bookingbusiness_list_services.md)や[予約状況](../api-reference/beta/api/bookingbusiness_post_appointments.md)を確認できます。 

業務担当者は、どこにいても Web、モバイル アプリ、対面、電話により予約を受け付けることができます。 既存の予約の[変更](../api-reference/beta//api/bookingappointment_update.md)、[キャンセル](../api-reference/beta/api/bookingappointment_cancel.md)、または別のスタッフ メンバーへの[再割り当て](../api-reference/beta/api/bookingappointment_update.md)を実行できます。 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>予約不履行が少なくなり、スタッフの生産性が向上する
事業担当者は予約やキャンセルに関する最低限の通知を含む[スケジュール ポリシー](../api-reference/beta/resources/bookingschedulingpolicy.md)を指定することができます。一方、顧客は、予約を入れたり変更したりする作業を自分で実行できます。 顧客からの予約確認や事業者側からの予約確認が自動化されるため、予約不履行が少なくなり、スタッフは自分の勤務時間をより有効に利用することができます。 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>どんな場所にいても顧客情報や顧客との関係を管理できる
顧客がすでに[顧客リスト](../api-reference/beta/api/bookingbusiness_list_customers.md)に記載されているなら、予約履行のための確認が自動的になされます。また必要なら顧客の名前とメール アドレスがリストに[追加](../api-reference/beta/api/bookingbusiness_post_customers.md)されます。 これは、業務担当者が顧客との接触を保ち、定期的にお知らせや販売促進資料を送付する上で便利です。

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Microsoft Graph での生産性向上およびチーム コラボレーション サービスの統合
同じ Microsoft Graph REST 統一エンドポイントを使用することにより、Bookings API にアクセスし、[Microsoft 365 の優れた機能を統合](overview-major-services.md)することにより、豊富なシナリオをサポートすることができます。 たとえば [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) を使用して事業の財務データを追跡および分析し、本格的なレポートを生成したり、[SharePoint](sharepoint-concept-overview.md) や [Microsoft Teams](teams-concept-overview.md) を使用してチーム コラボレーションを推進したりできます。

## <a name="next-steps"></a>次の手順

次の詳細情報をご確認ください:

- [Microsoft Bookings](https://support.office.com/en-us/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) およびその他の [Office 365 ビジネス アプリ](https://support.office.com/en-us/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US)。
- Microsoft Graph における [Bookings API の利用](../api-reference/beta/resources/booking-api-overview.md)。

