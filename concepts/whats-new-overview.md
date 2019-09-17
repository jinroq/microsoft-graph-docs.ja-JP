---
title: Microsoft Graph の新機能
description: Microsoft Graph の最新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 7a6ab3c50fe14986744ccfd64fdddadd9aa67a6e
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822775"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph の新機能

Microsoft Graph の一部の新機能は、開発者コミュニティでの要望が高かったことがきっかけとなり提供されるようになりました。 

Microsoft Graph チームでは、お客様のニーズを定期的に評価して、次の順序で新機能をリリースします。

1. **_プレビュー_** ステータスでデビューします。 関連するすべての REST API の更新プログラムは、ベータ版のエンドポイントに含まれます(`https://graph.microsoft.com/beta`)。  

2. フィードバックで十分に実行可能性が示されるようであれば、 **_一般提供_ (GA)** ステータスに昇格させます。 関連するすべての REST API の更新プログラムは、v1.0 エンドポイントに追加されます (`https://graph.microsoft.com/v1.0`)。 

以下は、Microsoft Graph の最新機能の特長、[アイデアの共有](#want-to-stay-in-the-loop)方法を示します。 API の更新の詳細については、API 変更ログの「[9 月](changelog.md#september-2019)」と「[8 月](changelog.md#august-2019)」のセクションを参照してください。 


## <a name="september-2019-new-in-preview"></a>2019 年 9 月: プレビューの新機能

> [!IMPORTANT]
> _プレビュー_ ステータスの機能 (API やツールを含む) は予告なしに変更されることがあり、一部の機能は GA ステータスに昇格されずに終わります。 製品版アプリにそれらの機能を使用しないでください。

### <a name="users"></a>ユーザー
- ユーザーが優先する[メールボックスの日付と時刻の形式設定](/graph/api/resources/mailboxsettings?view=graph-rest-beta)を取得または更新します。

## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月: 新機能および一般公開 

### <a name="reports"></a>レポート
- 削除されたアイテムの数とサイズに関する追加の[メールボックス使用状況データ](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)を取得します。
- [グループ アクティビティの詳細を取得する](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)ときに Office 365 グループ ID を追跡します。
- [OneDrive 使用状況の計算の詳細](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) と [SharePoint サイトの使用状況の詳細](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0) を取得するときに、所有者のプリンシパル名を追跡します。
- [Office 365 サービス単位のユーザー カウントに関するレポートを取得する](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0) ときに、Office 365 のアクティブなユーザーと非アクティブなユーザーの数を取得します。

### <a name="security"></a>セキュリティ
- 多数のパートナー企業の製品から Splunk へのセキュリティのアラートと分析情報をストリームするための新しい[ Splunk 向け Microsoft Graph Security API アドオン](https://aka.ms/graphsecuritysplunkaddon)を使用して、簡単にそれらのセキュリティ データのリアルタイムの相関関係を有効化します。 詳細については、[お知らせ](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972)を参照してください。 
- セキュリティ API で接続して統一された形式のデータを操作できるように、Microsoft または Microsoft パートナーによってビルドされた[その他のソリューションとコネクタの一覧を参照してください](security-integration.md)。


## <a name="august-2019-new-in-preview"></a>2019 年 8 月: プレビューの新機能

> [!IMPORTANT]
> _プレビュー_ ステータスの機能 (API やツールを含む) は予告なしに変更されることがあり、一部の機能は GA ステータスに昇格されずに終わります。 プレビュー ステータスの機能は製品版アプリでは使用しないでください。

### <a name="devices-and-apps"></a>デバイスとアプリ
Intune の [8 月](changelog.md#august-2019) の更新プログラム

### <a name="education"></a>教育
- 課題の特質とレベルで構成される[評価ルーブリック](/graph/api/resources/educationrubric?view=graph-rest-beta)に [教師](/graph/api/resources/educationuser?view=graph-rest-beta) または [課題](/graph/api/resources/educationassignment?view=graph-rest-beta)を関連付けます。 質の例にはスペルと文法が含まれます。レベルの例には "良い" と "悪い" が含まれます。 さらに、ルーブリックに得点と重みを関連付けることができます。 詳細については、 「[教育機関ルーブリックの概要](education-rubric-overview.md)」を参照してください。
- [フィードバック](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta)、[数値での評価](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta)、または[ルーブリック](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta)の観点から、課題を評価して結果を提示します。

### <a name="files"></a>ファイル
現時点まででは、[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) を [フォロー](/graph/api/driveitem-follow?view=graph-rest-beta)して、便利なアクセスを提供したり、移動、転送、名前を付けて保存などの操作を容易にしたりすることができます。 [フォローを取り消す](/graph/api/driveitem-unfollow?view=graph-rest-beta) アクションを使用して、ドライブ アイテムなどをフォローするのを停止できるようになりました。

### <a name="identity-and-access"></a>ID とアクセス
- 役割ベースのアクセス制御 (RBAC) のプロバイダーは、特定のリソースで実行される可能性がある[ロールのアクションを定義](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta)して Azure Active Directory で[ロールの管理](/graph/api/resources/rolemanagement?view=graph-rest-beta)をしたり、そうしたロールの定義に基づいて[ロールの割り当て](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta)を行い、それらのリソースに対応するアクセス権をそれらのロールに付与したりできます。
- 管理者は、グループ メンバーシップのレビューの効率的な円滑化、エンタープライズ アプリケーションへのアクセス、およびロールの割り当てを行うために、[アクセス レビューを一覧表示](/graph/api/accessreview-list?view=graph-rest-beta)することができます。 定期的なアクセス レビューにより、適切なユーザーのみ、特定のリソースに引き続きアクセスすることを確実にします。

### <a name="social-and-workplace-intelligence"></a>ソーシャル インテリジェンスおよび職場のインテリジェンス
エンド ユーザーは、Office 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) アプリを使用して、時間の管理、職場での共同作業、ワークライフバランスに関する分析情報を取得できます。 現在、通話、チャット、メールなどの作業活動に費やされる時間のデータを統合したり、ユーザーの生産性とウェルビーイングを向上させたりするための[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns)を使用できるようになりました。 


## <a name="want-to-stay-in-the-loop"></a>常に最新の情報を把握するには
- Microsoft Graph でのサポートを希望するシナリオがある場合は、 [Microsoft Graph User Voice (Microsoft Graph のユーザーの声)](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) で新機能の提案と投票を行ってください。
- Microsoft Graph コミュニティで活発に活動してください。 毎月の Microsoft Graph コミュニティ コールに[参加](https://aka.ms/microsoftgraphcall)してみてください。
- [Office 365 開発者プログラム](https://developer.microsoft.com/ja-JP/office/dev-program)に登録すると、Office 365 サブスクリプションを無料で入手し、開発を開始できます。


## <a name="see-also"></a>関連項目
- リリース告知と役立つリソースについては、「[Microsoft Graph developer blog (Microsoft Graph 開発者ブログ)](https://developer.microsoft.com/en-us/graph/blogs/)」を定期的に確認してください。
- Microsoft Graph API の追加機能や API 動作の更新内容の詳細については、「[changelog](changelog.md)」を参照してください。
- 「[以前のリリースでの主な変更点](whats-new-earlier.md)」をご覧ください。
- 詳細については、「[Microsoft Graph のバージョン管理、サポートと重大な変更の方針](versioning-and-support.md)」を参照してください。

