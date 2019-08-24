---
title: Microsoft Graph の新機能
description: Microsoft Graph の最新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 57a1ce3ac96577b31d1f5120dc3d88e89e288bd1
ms.sourcegitcommit: 0d57eda47899baacc95385e331979880e069fba9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36564742"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph の新機能

Microsoft Graph の一部の新機能は、開発者コミュニティでの要望が高かったことがきっかけとなり提供されるようになりました。 

Microsoft Graph チームでは、お客様のニーズを定期的に評価して、次の順序で新機能をリリースします。

1. **_プレビュー_** ステータスでデビューします。 関連するすべての REST API の更新プログラムは、ベータ版のエンドポイントに含まれます(`https://graph.microsoft.com/beta`)。  

2. フィードバックで十分に実行可能性が示されるようであれば、 **_一般提供_ (GA)** ステータスに昇格させます。 関連するすべての REST API の更新プログラムは、v1.0 エンドポイントに追加されます (`https://graph.microsoft.com/v1.0`)。 

以下は、Microsoft Graph の最新機能の特長、[アイデアの共有](#want-to-stay-in-the-loop)方法を示します。 API の更新の詳細については、API 変更ログの「[8 月](changelog.md#august-2019)」と「[7 月](changelog.md#july-2019)」のセクションを参照してください。 


## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月: 新機能および一般公開 

### <a name="reports"></a>レポート
- 削除されたアイテムの数とサイズに関する追加の[メールボックス使用状況データ](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)を取得します。
- [グループ アクティビティの詳細を取得する](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)ときに Office 365 グループ ID を追跡します。
- [OneDrive 使用状況の計算の詳細](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) と [SharePoint サイトの使用状況の詳細](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0) を取得するときに、所有者のプリンシパル名を追跡します。
- [Office 365 サービス単位のユーザー カウントに関するレポートを取得する](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0) ときに、Office 365 のアクティブなユーザーと非アクティブなユーザーの数を取得します。


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
[MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) は、時間の管理、職場での共同作業、ワークライフバランスに関するエンド ユーザーの分析情報を提供する Office 365 アプリです。 通話、チャット、メールなどの作業活動に費やされる時間のデータを統合したり、ユーザーの生産性とウェルビーイングを向上させたりするための[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns)を使用できるようになりました。 

## <a name="july-2019-new-and-generally-available"></a>2019 年 7 月: 新機能および一般公開 

### <a name="example-code-snippets"></a>コード スニペットの例
v1.0 およびベータ リファレンスのすべての API トピックに、Objective-C のコード スニペットが含まれるようになりました。 [イベントを取得](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)するための、Objective-C の例をご覧ください。

### <a name="group"></a>グループ
- [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) 関数を使用して、既存の Office 365 グループの表示名またはメールニックネームが命名ポリシーに準拠していることを確認します。
- または、グループを作成する前に、[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) の [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) 関数を使用して、最初に名前を検証できます。

### <a name="identity-and-access"></a>ID とアクセス
- [新しい委任されたアクセス許可およびアプリケーション アクセス許可](permissions-reference.md#organization-permissions)、_Organization.Read.All_、ならびに _Organization.ReadWrite.All_ を使用して[組織](/graph/api/resources/organization?view=graph-rest-1.0)や [購読している SKUs](/graph/api/resources/subscribedsku?view=graph-rest-1.0) などの関連リソースにアクセスします。
- 会社のディレクトリの役割ベースのアクセス制御（RBAC）には、[新しい委任およびアプリケーションの権限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ および_RoleManagement.ReadWrite.Directory_ を使用します。

  - 読み取り/書き込み権限を使用して、最初にディレクトリ ロールを[アクティブ化](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0)します。 
  - ロールをアクティブにすると、読み取り権限を使用して、[ディレクトリ ロールの読み取り](/graph/api/directoryrole-list?view=graph-rest-1.0)、[ロールメンバーの一覧表示](/graph/api/directoryrole-list-members?view=graph-rest-1.0)、および[ディレクトリ ロール テンプレートの一覧表示](/graph/api/directoryroletemplate-list?view=graph-rest-1.0)ができます。 
  - また、読み取り/書き込み権限を使用して、ロール メンバーを[追加](/graph/api/directoryrole-post-members?view=graph-rest-1.0)したり、[削除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0)したりすることができます。


## <a name="july-2019-new-in-preview"></a>2019 年 7 月: プレビューの新機能

> [!IMPORTANT]
> _プレビュー_ ステータスの機能 (API やツールを含む) は予告なしに変更されることがあり、一部の機能は GA ステータスに昇格されずに終わります。 製品版アプリにそれらの機能を使用しないでください。

### <a name="calendar"></a>カレンダー 
新しい [places API](/graph/api/resources/place?view=graph-rest-beta) を使用して、Exchange Online 管理者が設定した[部屋](/graph/api/resources/room?view=graph-rest-beta)や[部屋リスト](/graph/api/resources/roomlist?view=graph-rest-beta)などの豊富なロケーション タイプを活用できます。

### <a name="devices-and-apps"></a>デバイスとアプリ
Intune [7 月](changelog.md#july-2019)の更新プログラム

### <a name="files"></a>ファイル 
ファイル、フォルダー、またはその他の [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) の[共有リンクの作成](/graph/api/driveitem-createlink?view=graph-rest-beta)を行うときに、有効期限の日時またはパスワードを適用します。

### <a name="identity-and-access"></a>ID とアクセス
- [アクセス レビュー](/graph/api/resources/accessreviews-root?view=graph-rest-beta) の CRUD 操作のための [新しいアプリケーションのアクセス許可](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ を使用します。 
- [新しい委任およびアプリケーションの権限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_、および_AdministrativeUnit.ReadWrite.All_ を使用して、それぞれの[管理ユニット](/graph/api/resources/administrativeunit?view=graph-rest-beta) リソースの読み取りまたは書き込みを行います（作成、更新、削除、またはメンバーシップの管理を含む）。
- [新しい委任されたアクセス許可およびアプリケーション アクセス許可](permissions-reference.md#organization-permissions)、_Organization.Read.All_ および _Organization.ReadWrite.All_ を使用して、[組織](/graph/api/resources/organization?view=graph-rest-beta) や [購読している SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta) などの関連リソースにアクセスします。
- 新しい[discover](/graph/api/directorydefinition-discover?view=graph-rest-beta) 関数を使用して最新のディレクトリ[同期スキーマ](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)を検索し、ディレクトリ オブジェクト、属性、それらの種類をアプリに同期します。
- [機能ロールアウト ポリシー](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta) を使用して、テナント管理者が機能を組織全体で有効にする前に、特定のグループに対して試験運用を実施するのを助けます。

### <a name="mail"></a>メール
より詳細なアプリケーション アクセス許可、_Mail.ReadBasic.All_ を使用して、メッセージ本文、プレビュー本文、添付ファイルを除くユーザーのメールボックスと、メールボックスの検索を除く拡張プロパティを読み取ります。 [message](/graph/api/resources/message?view=graph-rest-beta) と **mailFolder**用の[mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) と [変更履歴](delta-query-overview.md) に適用できるようになりました。

### <a name="reports"></a>レポート
- 削除されたアイテムの数とサイズに関する追加の[メールボックス使用状況データ](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)を取得します。

### <a name="teamwork"></a>チームワーク
- ユーザーのための[インストール](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)、[アンインストール](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta)、[アップグレード](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)、および[インストール済みの Microsoft Teams アプリの一覧表示](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta)を行います。
- アプリのみのアクセスを使用して、チャンネルメッセージ、チャンネルメッセージへの返信、チャット内のメッセージを読み取ります。 そのようなアクセス権の[要求と承諾](teams-protected-apis.md)を得ます。

## <a name="want-to-stay-in-the-loop"></a>常に最新の情報を把握するには
- Microsoft Graph でのサポートを希望するシナリオがある場合は、 [Microsoft Graph User Voice (Microsoft Graph のユーザーの声)](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) で新機能の提案と投票を行ってください。
- Microsoft Graph コミュニティで活発に活動してください。 毎月の Microsoft Graph コミュニティ コールに[参加](https://aka.ms/microsoftgraphcall)してみてください。
- 
  [Office 365 開発者プログラム](https://developer.microsoft.com/ja-JP/office/dev-program)に登録すると、Office 365 サブスクリプションを無料で入手し、開発を開始できます。


## <a name="see-also"></a>関連項目
- リリース告知と役立つリソースについては、「[Microsoft Graph developer blog (Microsoft Graph 開発者ブログ)](https://developer.microsoft.com/en-us/graph/blogs/)」を定期的に確認してください。
- Microsoft Graph API の追加機能や API 動作の更新内容の詳細については、「[changelog](changelog.md)」を参照してください。
- 「[以前のリリースでの主な変更点](whats-new-earlier.md)」をご覧ください。
- 詳細については、「[Microsoft Graph のバージョン管理、サポートと重大な変更の方針](versioning-and-support.md)」を参照してください。

