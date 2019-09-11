---
title: Microsoft Graph の以前のリリースでの主な変更点
description: Microsoft Graph の以前の新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e2c20e4d39d5aafe71379553a566752451266bf2
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822803"
---
# <a name="highlights-of-earlier-releases"></a>以前のリリースでの主な変更点

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
- アプリのみのアクセスを使用して、チャンネルメッセージ、チャンネルメッセージへの返信、チャット内のメッセージを読み取ります。 そのようなアクセス権の[要求と承諾](teams-protected-apis.md)を取得します。

## <a name="may---june-2019-new-and-generally-available"></a>2019 年 5 月 - 6 月: 新機能および一般公開

### <a name="calendar-mail-and-personal-contacts"></a>予定表、メール、個人用連絡先
Exchange 管理者はアプリにアプリケーションのアクセス許可を付与することで、組織内のすべてのメールボックスへのアクセスを許可する既定のアクセス許可の代わりに、[アプリによるアクセスを組織内のメールボックスのサブセットのみに制限](auth-limit-mailbox-access.md)することができます。 このようなアクセス制限は、[予定表](permissions-reference.md#calendars-permissions)、[連絡先](permissions-reference.md#contacts-permissions)、[メールおよびメールボックスの設定](permissions-reference.md#mail-permissions)のアプリに付与されているアプリケーション アクセス許可すべてに適用されます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)を参照してください。

### <a name="mail"></a>メール
[メール検索フォルダー](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API を使用して、メッセージを検索し、Outlook のメール検索結果にアクセスできます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)を参照してください。

### <a name="postman"></a>Postman
API の動作を学習し、アプリ開発を高速化するために、Graph Explorer の代替として、[Microsoft Graph Postman コレクション](use-postman.md)で Microsoft Graph API をお試しください。

### <a name="tutorials"></a>チュートリアル
[Java コンソール アプリを作成するための新しいチュートリアル](/graph/tutorials/java)を試しに使用して、ユーザーの予定表に関する情報を入手してみてください。

### <a name="user"></a>ユーザー
管理者またはユーザーは、ユーザーに発行されたすべての更新トークンを[取り消す](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)ことができます。 この機能は通常、紛失または盗難にあったデバイスのアプリで組織のデータにアクセスされないようにするために使用されます。


## <a name="may---june-2019-new-in-preview"></a>2019 年 5 月 - 6 月: プレビューの新機能

> [!IMPORTANT]
> _プレビュー_ ステータスの機能 (API やツールを含む) は予告なしに変更されることがあり、一部の機能は GA ステータスに昇格されずに終わります。 プレビュー ステータスの機能は製品版アプリでは使用しないでください。

### <a name="devices-and-apps"></a>デバイスとアプリ
- Intune の[5 月](changelog.md#may-2019)の更新プログラム 
- Intune の[6 月](changelog.md#june-2019)の更新プログラム

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta) のデルタ クエリ。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) および [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta) のデルタ クエリと追加プロパティ。

### <a name="group"></a>グループ
[機密度ラベル](/graph/api/resources/assignedlabel?view=graph-rest-beta)を取得すると、Office 365 グループの機密データを保護し、コンプライアンス ポリシーを満たす目的に役立ちます。 これらのラベルは [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta) オブジェクトで、Microsoft Information Protection 機能の一部として、管理者が Microsoft 365 セキュリティ/コンプライアンス センターで公開します。 

### <a name="identity-and-access"></a>ID とアクセス
- [アプリケーション](/graph/api/resources/applicationtemplate?view=graph-rest-beta)のインスタンスを取得したり、Azure AD アプリケーション ギャラリーのインスタンスをテンプレートとしてディレクトリに追加したりできます。
- テナントにあるすべてのディレクトリ [プロビジョニング イベント](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)の記録を取得できます。
- Azure AD 環境で[検出されたユーザーまたはサインイン リスク](/graph/api/resources/riskdetection?view=graph-rest-beta)に関する情報を取得できます。 このリスク検出機能は、Azure AD Identity Protection の一部です。

### <a name="mail"></a>メール
より詳細な委任されたアクセス許可、_Mail.ReadBasic_ を使用して、メッセージ本文、プレビュー本文、添付ファイルを除くユーザーのメールボックスと、メールボックスの検索を除く拡張プロパティを読み取ります。 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) のメソッドを読み取り、[メッセージ](delta-query-overview.md)と [mailFolder](/graph/api/resources/message?view=graph-rest-beta) の**変更履歴**に使用できます。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph ツールキット
[Microsoft Graph ツールキット](/graph/toolkit/overview)とは、フレームワークに依存しない Web コンポーネントおよびヘルパーのセットで、Microsoft Graph でのデータの認証とアクセスを簡便にします。 Microsoft Graph ツールキットはプレビュー ステータスであるため、製品版以外のアプリでのみツールキットのプロバイダーとコンポーネントを使用してください。

### <a name="reports"></a>レポート
- セルフサービスによるパスワードのリセットや多要素認証 (MFA) など、組織内のユーザーによって導入される[認証方法に関するレポート](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta)を取得します。

### <a name="sites"></a>サイト
ユーザーは SharePoint サイトを[フォロー](/graph/api/site-follow?view=graph-rest-beta)または[フォロー解除](/graph/api/site-unfollow?view=graph-rest-beta)できます。

### <a name="teamwork"></a>チームワーク
- Microsoft Teams の[チャット メッセージ](/graph/api/resources/chatmessage?view=graph-rest-beta)の[画像](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)をホストできます。
- プライベート チームの検出方法の[構成](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)がサポートされます。


## <a name="january---april-2019-new-and-generally-available"></a>2019 年 1 月 - 4 月: 新機能および一般公開

[Microsoft Graph データ接続](data-connect-concept-overview.md)

### <a name="calendar"></a>カレンダー
[空き時間のスケジュールを取得する](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>ID とアクセス
[ID プロバイダー](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[改善された認証ガイド](/graph/auth)
[Azure AD Graph から Microsoft Graph へのアプリの移行](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>SDK
[SDK ガイド](/sdks/sdks-overview.md) API スニペット ([例](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code))

### <a name="security"></a>セキュリティ
[テナントのセキュア スコア](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>2019 年 1 月 - 4 日: プレビューの新機能

### <a name="calendar-group-mail-to-do-tasks"></a>カレンダー、グループ、メール、To-do タスク
イベント、メッセージ、Outlook タスク、グループ投稿での、[添付アイテムまたは添付ファイルの raw/MIME コンテンツの取得](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)

### <a name="change-notifications"></a>変更通知
[Outlook リソースの変更通知の見逃しを減らす](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>デバイスとアプリ
- Intune [1 月](changelog.md#january-2019)の更新プログラム 
- Intune [2 月](changelog.md#february-2019)の更新プログラム
- Intune [3 月](changelog.md#march-2019)の更新プログラム
- Intune [4 月](changelog.md#april-2019)の更新プログラム

### <a name="files"></a>ファイル
有効期限とパスワードを含めることができるようになった[共有の招待](/graph/api/driveitem-invite?view=graph-rest-beta)

### <a name="financials"></a>財務報告
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>ID とアクセス
[アクセス レビュー](/graph/api/resources/accessreviews-root?view=graph-rest-beta) アプリケーション アクセス許可のサポート [監査とサインイン ログ](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Azure AD B2C でのカスタム サインインとサインアップ](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[リスクの高いユーザー](/graph/api/resources/riskyuser?view=graph-rest-beta) および [履歴](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>メール
[メッセージの MIME コンテンツを取得する](outlook-get-mime-message.md)

### <a name="reports"></a>レポート
[アプリケーションのサインイン レポート](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>セキュリティ
[セキュリティ アクション](/graph/api/resources/securityaction?view=graph-rest-beta)
[脅威インジケーター](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>チームワーク
[1:1 のチャット](/graph/api/resources/chat?view=graph-rest-beta)
[シフト管理](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>関連項目
- Microsoft Graph の[最新機能](whats-new-overview.md)を参照してください。
- リリース告知と役に立つリソースについては、「[Microsoft Graph 開発者ブログ](https://developer.microsoft.com/en-us/graph/blogs/)」を定期的に確認してください。
- Microsoft Graph API の追加機能、[更新ログ](changelog.md)の API 動作の更新内容の詳細を参照してください。