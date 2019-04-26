---
title: Microsoft Graph レポート API の概要
description: Microsoft 365 管理センターの使用状況レポートを利用することにより管理者は、会社における Office 365 のサービスの利用状況を理解することができます。 Microsoft Graph のレポート API を使用することにより、Office 365 使用状況レポートと統合することができます。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 44b1b7f2c236ef54c7a674f5421c2978e34aeb73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564128"
---
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
|Microsoft Teams|[デバイスの使用状況](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>|[ユーザー アクティビティ](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0)|
|Office 365 (標準) |[アクティブ化](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[アクティブなユーザー](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[グループのアクティビティ](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0)|
|OneDrive |[アクティビティ](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[使用状況](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0)|
|Outlook|[アクティビティ](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[アプリの使用状況](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[メールボックス使用状況](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0)|
|SharePoint |[アクティビティ](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[サイトの使用状況](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0)|
|Skype for Business |[アクティビティ](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[デバイスの使用状況](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[デバイスの使用状況](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[参加者のアクティビティ](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[ピア ツー ピア アクティビティ](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0)|
|Yammer |[アクティビティ](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[デバイスの使用状況](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[グループのアクティビティ](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0)|

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Office 365 使用状況レポート API](/graph/api/resources/report?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Office 365 使用状況レポート API](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

* [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) の API について調べる
* [レポート REST API の使用](/graph/api/resources/report?view=graph-rest-1.0)方法の詳細を確認する
