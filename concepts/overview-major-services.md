---
title: Microsoft Graph の主要なサービスおよび機能
description: 'Microsoft Graph では、REST API とクライアント ライブラリを使用して、非常に優れた Office 365、Windows 10、および Microsoft 365 の Enterprise Mobility and Security のサービスを統合することができます。 さらに、ユーザーの生産性、創造性、チーム共同作業を促進し、ビジネス リソースおよびユーザー データを保護することのできるセキュリティおよびソーシャル インテリジェンスが提供されます。 '
author: jthake-msft
ms.openlocfilehash: 6f4403db3179afadb39dfb20613f284381650112
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353551"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Microsoft Graph の主要なサービスおよび機能

Microsoft Graph では、REST API とクライアント ライブラリを使用して、非常に優れた Office 365、Windows 10、および Microsoft 365 の Enterprise Mobility and Security のサービスを統合することができます。 さらに、ユーザーの生産性、創造性、チーム共同作業を促進し、ビジネス リソースおよびユーザー データを保護することのできるセキュリティおよびソーシャル インテリジェンスが提供されます。 

## <a name="users-and-groups"></a>ユーザーとグループ

Microsoft Graph の中心となるのは、ユーザーおよびグループの概念です。 

Microsoft Graph の_ユーザー_は、Microsoft 365 クラウド サービスを使用する何百万人のうちの 1 人です。 これは、ID が保護され、アクセスが的確に管理されるフォーカル ポイントです。 ユーザーのデータは、ビジネスを推進する力となるものです。 Microsoft Graph サービスによりそのデータが、豊富なコンテキスト、リアルタイムの更新、および深い洞察において企業から利用可能になり、しかも常に適切な許可によってのみ利用可能になります。

Office 365 の_グループ_は、ユーザーが共同作業を実行するための基本的なエンティティです。 これは、他のサービスと統合して、タスク計画、共同作業、教育などにおいて豊富なシナリオが可能になります。 

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| ユーザー | Azure AD および生産性向上、コラボレーション、インテリジェンス、および教育機関向けの多くのサービス | ユーザーは、Microsoft Graph の中心となるものであり、多くの Microsoft Graph サービスは、ユーザー中心の機能を構築します。 | [Microsoft Graph でのユーザーの概要](azuread-users-concept-overview.md)|
|グループ | Azure AD、OneDrive、OneNote、Outlook、Planner | Office 365 グループは、ユーザーが会話、ファイル、メモ、予定表、プランなどを共有するための基本コラボレーション単位を提供します。 | [Microsoft Graph での Office 365 グループの概要](office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>ユーザーのデータ、Microsoft 365 サービス、およびアプリの接続

中心となるユーザーおよびグループを始めとして、Microsoft Graph は、広範囲に及ぶシナリオをサポートするためのデータを管理、保護、および抽出する Microsoft 365 のサービスと機能のネットワークを形成します。 Microsoft Graph により、当人の承認を尊重しながら、豊富なユーザー データにアクセスすることができます。

![Microsoft Graph からユーザーのデータに接続する](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>サービスと機能

Microsoft Graph の一部のサービスは、そこで初めて登場したサービスであり、その他のサービスはスタンドアロン サービスとして知られており、現在 Microsoft Graph に収束しています。 その API セットは、「[Microsoft REST API ガイドライン](https://github.com/Microsoft/api-guidelines)」で詳細が示されている合理化デザインに従うものであり、Microsoft Graph REST の単一エンドポイントによってアクセス可能になっています。`https://graph.microsoft.com` この記事の残りの部分では、主要なサービスと機能をカテゴリ別に一覧表示します。 


## <a name="identity-and-access-management"></a>ID およびアクセス管理

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| ID およびアクセス管理 | Azure AD | ユーザー、グループ、およびアプリケーションなどのディレクトリ リソースを作成したり管理したりします。 リソースおよびデータへのアクセスを管理します。 Azure AD 内のサインインおよびアカウント リスク データへのアクセス権をユーザーに付与します。| [Azure AD ID およびアクセス管理の概要](azuread-identity-access-management-concept-overview.md)  |


## <a name="productivity"></a>生産性

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| 予定表 | Outlook  | ユーザーが、Web、モバイル、およびデスクトップ デバイスの上で予定と会議を設定することができるようにします。 これは、Office 365 の中の Outlook メッセージング通信ハブの一部であり、それにより、ユーザーはメールと連絡先を管理することができます。 | [Outlook カレンダーの概要](outlook-calendar-concept-overview.md)  |
| ファイル | OneDrive と SharePoint | OneDrive および SharePoint でユーザー ファイルを管理および共有します。 | [OneDrive ファイル ストレージの概要](onedrive-concept-overview.md) |
| メール | Outlook | ユーザーが、ワークフローの中で、Web、モバイル、およびデスクトップ デバイス上で、通信したり、メッセージを整理したり、優先順位を管理したりできるようにします。 これは、Office 365 の中の Outlook 通信ハブの一部であり、それにより、ユーザーは連絡先を管理したり、会議をスケジューリングしたりできます。 | [Outlook メールの概要](outlook-mail-concept-overview.md) |
| メモ | OneNote | ユーザーが、アイデアと情報を計画したり整理したりできるようにします。 | [OneNote ノートの概要](integrate-with-onenote.md) |
| 個人用連絡先 | Outlook | Web、モバイル、およびデスクトップ デバイス上での連絡先マネージャー。 これは、Office 365 の中の Outlook メッセージング通信ハブの一部であり、それにより、ユーザーはメールを管理したり、会議をスケジューリングしたりすることができます。  | [Outlook 個人用連絡先の概要](outlook-contacts-concept-overview.md) |
| ブックとグラフ | Excel | ユーザーが Excel のスプレッドシートを使用して、複雑な計算を実行したり、データを追跡、分析、および視覚化したり、本格的なレポートを生成したりできるようにします。 | [Excel のブックとグラフの概要](excel-concept-overview.md) |


## <a name="collaboration"></a>グループ作業

<!-- Want to update links to concept overviews as they are created over time. 
-->
|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| サイトとリスト  | SharePoint | ユーザーおよび Office 365 グループがコンテンツ (リスト、ファイル、ノートを含む) を共有、整理、管理、および検出するための Web ベースのプラットフォーム。 | [SharePoint のサイトおよびコンテンツの概要](sharepoint-concept-overview.md) | 
|タスクとプラン | Planner | Office 365 グループ内のユーザーがプランを作成したり、タスクを割り当てたり、進捗状況を追跡したりできるようにします。 | [Planner のプランとタスクの概要](planner-concept-overview.md) |
|チームワーク |  Microsoft Teams | チームがファイル、ノート、予定表、およびプランを共有するための、デジタル ハブおよびチャット ベースのワークスペース。 | [Microsoft Teams のチームワークの概要](teams-concept-overview.md) |


## <a name="social-intelligence-and-analytics"></a>ソーシャル インテリジェンスおよび分析機能

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| ソーシャル インテリジェンス: 連絡先 | Azure AD、Outlook、SharePoint など | ユーザーの通信や共同作業のパターン、またビジネスの付き合いによって決まるユーザーとの関連性に応じて連絡先についての情報を取得します。  | [Microsoft Graph でのソーシャル インテリジェンス](social-intel-concept-overview.md) |
| ソーシャル インテリジェンス: ドキュメントのインサイト (プレビュー) | Delve、OneDrive、Outlook、SharePoint | 高度な分析機能と機械学習のテクニックを使用して、よく使用されるドキュメントやユーザーが表示、変更、または共有したドキュメントを取得します。  | [Microsoft Graph でのソーシャル インテリジェンス](social-intel-concept-overview.md)  |


## <a name="device-management"></a>デバイスの管理

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
|デバイスとアプリ | Intune | デバイスを登録および構成し、組織内でモバイル アプリケーション管理します。 | [Intune のデバイスとアプリの概要](intune-concept-overview.md) |


## <a name="security"></a>セキュリティ

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| セキュリティ統合 | Azure AD Identity Protection、Azure Information Protection、Azure Security Center、Microsoft Cloud Application Security、Windows Defender Advanced Threat Protection、[その他](/graph/api/resources/security-api-overview?view=graph-rest-1.0) | Microsoft およびエコシステムのパートナーを通じて、セキュリティの分析情報やアクションに対する統一ゲートウェイを提供します。 | [Microsoft Graph のセキュリティ](security-concept-overview.md) |



## <a name="cross-device-experiences"></a>クロスデバイス エクスペリエンス

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| クロスデバイス エクスペリエンス | アクティビティ フィード、デバイスの中継 | 単一デバイスを超えて、種類やプラットフォームに関係なくデバイスからデバイスへユーザーと共に移行できるアプリ エクスペリエンスを可能にします。 | [クロスデバイス エクスペリエンスの概要](cross-device-concept-overview.md) |


## <a name="usage-reports"></a>利用状況レポート

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| レポート | Microsoft Teams、OneDrive、Outlook、SharePoint、Skype for Business、Yammer | サポート サービスのアクティビティおよび使用状況の情報を取得します。 | [使用状況レポートの概要](reportroot-concept-overview.md) |


## <a name="education"></a>教育

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| 教育 | Azure AD、教育 | 学校、クラス、学生、教師、および割り当て情報など、教育機関向けシナリオに関連する情報を提供します。 ISV が、教師の作業時間を短縮し、チームワークとコラボレーションを促進する教室用のアプリケーションをビルドできるようにします。  | [教育機関向けの概要](education-concept-overview.md) |


## <a name="business-applications"></a>ビジネス アプリケーション

|機能     |サポートするサービス  |説明 |詳細情報 |
|:-----------|:--------------------|:-----------|:----------------|
| 顧客の予約 (プレビュー) | Microsoft Bookings | 小規模企業を対象として、顧客が Web または Facebook 上で直接にサービスを予約できるようにします。 業務担当者が、顧客の好み、サービスと価格、スタッフのリストとスケジュール、その他の一般的なビジネス情報を管理できるようにします。 | [Microsoft Bookings API の概要](booking-concept-overview.md) |


## <a name="next-steps"></a>次の手順

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- 実際の顧客の問題を解決する、Microsoft Graph のサービスに基づいて構築されたクリエイティブなソリューションの[例](https://developer.microsoft.com/graph/examples)を参照してください。
- 目次の「**詳細情報**」を見て、さまざまなシナリオで使用できるサービスや機能についての詳細情報を参照します _。_
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)でサンプルの要求を試します。
- [クイック スタート](https://developer.microsoft.com/graph/quick-start)を使用して、すぐに実行できるサンプル アプリをセットアップします。
