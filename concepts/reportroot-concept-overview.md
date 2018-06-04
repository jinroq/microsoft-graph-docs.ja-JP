# <a name="microsoft-graph-reports-api-overview"></a>Microsoft Graph レポート API の概要

Microsoft 365 管理センターの使用状況レポートを利用することにより管理者は、会社における Office 365 のサービスの利用状況を理解することができます。 Microsoft Graph のレポート API を使用することにより、Office 365 使用状況レポートと統合することができます。

## <a name="why-use-the-reports-api"></a>レポート API を使用する理由

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Office 365 使用状況レポート作成機能を組織の既存のレポート作成ソリューションに統合する
多くの会社には、レポート作成アプリケーションや Web ポータルを使用する既存のレポート作成ソリューションがあります。 レポート API を使用して Office 365 の使用状況データを、組織の既存のレポート作成ソリューションに統合することにより、すべての IT サービス レポートを 1 つの統合場所にまとめることができます。  

### <a name="retain-usage-reports-for-historical-analysis"></a>履歴分析用に使用状況レポートを保持する
レポート API を使用することにより、サービスごとの組織レベルでの要約、最後の 7/30/90/180 日間についてのエンティティ レベル (ユーザー、サイト、アカウント) の使用状況情報、および毎日の活動集計など、あらゆる使用状況レポートで利用可能なデータを入手できます。 これにより、必要に応じて使用状況履歴情報を保持するオプションが提供されます。

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>レポート API を使用してアクセスできるデータ

レポート API を使用することにより、次の表に記載されているデータ セットにアクセスすることができます。

|Office 365 アプリ|データ セット|
|:--------|:--------|
|Microsoft Teams|[デバイスの使用状況](../api-reference/v1.0/resources/microsoft_teams_device_usage_reports.md)<br/>|[ユーザー アクティビティ](../api-reference/v1.0/resources/microsoft_teams_user_activity_reports.md)|
|Office 365 (標準) |[アクティブ化](../api-reference/v1.0/resources/office_365_activations_reports.md)<br/>[アクティブなユーザー](../api-reference/v1.0/resources/office_365_active_users_reports.md)<br/>[グループのアクティビティ](../api-reference/v1.0/resources/office_365_groups_activity_reports.md)|
|OneDrive |[アクティビティ](../api-reference/v1.0/resources/onedrive_activity_reports.md)<br/>[使用状況](../api-reference/v1.0/resources/onedrive_usage_reports.md)|
|Outlook|[アクティビティ](../api-reference/v1.0/resources/email_activity_reports.md)<br/>[アプリの使用状況](../api-reference/v1.0/resources/email_app_usage_reports.md)<br/>[メールボックス使用状況](../api-reference/v1.0/resources/mailbox_usage_reports.md)|
|SharePoint |[アクティビティ](../api-reference/v1.0/resources/sharepoint_activity_reports.md)<br/>[サイトの使用状況](../api-reference/v1.0/resources/sharepoint_site_usage_reports.md)|
|Skype for Business |[アクティビティ](../api-reference/v1.0/resources/skype_for_business_activity_reports.md)<br/>[デバイスの使用状況](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[デバイスの使用状況](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[参加者のアクティビティ](../api-reference/v1.0/resources/skype_for_business_participant_activity_reports.md)<br/>[ピア ツー ピア アクティビティ](../api-reference/v1.0/resources/skype_for_business_peer_to_peer_activity.md)|
|Yammer |[アクティビティ](../api-reference/v1.0/resources/yammer_activity_reports.md)<br/>[デバイスの使用状況](../api-reference/v1.0/resources/yammer_device_usage_reports.md)<br/>[グループのアクティビティ](../api-reference/v1.0/resources/yammer_groups_activity_reports.md)|

## <a name="next-steps"></a>次の手順

* [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) の API について調べる
* [レポート REST API の使用](../api-reference/v1.0/resources/report.md)方法の詳細を確認する
