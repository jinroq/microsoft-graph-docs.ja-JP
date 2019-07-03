---
title: Microsoft Graph の新機能
description: Microsoft Graph の最新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 416ba84527957b59ad4f8ff9e6d8c0194d60f245
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35420439"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph の新機能

Microsoft Graph の新機能の一部は、開発者コミュニティから人気のある要求として発信されていることを知っていましたか? 

では、新機能の基本的なライフ サイクル、Microsoft Graph の最新機能や[アイデアの共有](#want-to-stay-in-the-loop)方法について見ていきましょう。

## <a name="life-cycle-of-a-feature"></a>機能のライフ サイクル

Microsoft Graph サービスの所有者は、機能のアイデアや顧客のニーズを定期的に評価し、サポートする新しいシナリオを選択します。 新機能を作成するために、REST API を追加または更新することがあります。 API 構文を同じにして、機能の動作を拡張する場合があります。 あるいは、学習または開発環境を改善することがあります。

ほとんどの場合、サービス所有者は次の順序で新機能をリリースします。

1. **_「プレビュー」_** 状態のデビューとは、機能の動作が予告なく変更される可能性があるということです。 所有者は、beta エンドポイント (`https://graph.microsoft.com/beta`) で関連する REST API の追加や更新プログラムを公開します。 製品版アプリでは、API を含むプレビュー機能を使用しないでください。

2. サービスの所有者がフィードバックを十分に受け取り、その機能を使用できると判断した場合、所有者は機能を**_「一般提供」_(GA)** 状態にします。 この所有者は、v1.0 エンドポイント (`https://graph.microsoft.com/v1.0`) に関連する API の追加や更新プログラムも加えます。 (APIを含む) この機能は、製品版アプリの GA 状態で使用できます。

以下のセクションでは、2019 年 5 月と 6 月の新機能について説明します。 API の更新プログラムの詳細については、changelogの [5 月](changelog.md#may-2019)と [6 月](changelog.md#june-2019) のセクションを参照してください。 

## <a name="new-and-generally-available-released-may---june-2019"></a>新機能と一般公開 (2019 年 5 月～6 月にリリース済み)

### <a name="calendar-mail-and-personal-contacts"></a>予定表、メール、個人の連絡先
Exchange 管理者はアプリケーションにアプリのアクセス許可を付与し、[組織内のすべてのメールボックスへのアクセスであるデフォルトではなく、](auth-limit-mailbox-access.md)内のメールボックスのサブセットのみにアクセスするようにアプリを制限できます。 こういったアクセス制限は、[予定表](permissions-reference.md#calendars-permissions)、[連絡先](permissions-reference.md#contacts-permissions)、[メールとメールボックス設定](permissions-reference.md#mail-permissions)のアプリに付与されているアプリケーションのアクセス許可に適用されます。 関連する「[ブログのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)」を参照してください。

### <a name="example-code-snippets"></a>コード スニペットの例
C# と JavaScript に加えて、v1.0 およびベータ リファレンスのすべての API トピックに Objective-C のコード スニペットが用意されています。 [イベントを取得する](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)には、Objective-C の例を参照してください。

### <a name="mail"></a>メール
[メール検索フォルダー](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API を使用して、メッセージを検索し、Outlook のメール検索結果にアクセスします。 関連する「[ブログのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)」を参照してください。

### <a name="postman"></a>Postman
Graph Explorer の代わりに、 [Microsoft Graph Postman コレクション](use-postman.md)で Microsoft Graph API を試して API の動作を学習し、アプリの開発を高速にします。

### <a name="tutorials"></a>チュートリアル
[Java コンソール アプリを作成するのに新しいチュートリアルを試し](/graph/tutorials/java)、ユーザーの予定表に関する情報を入手してください。

### <a name="user"></a>ユーザー
管理者またはユーザーが、ユーザー向けに発行されたすべての更新トークンを[取り消します](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)。 通常は、デバイスの紛失または盗難時、組織のデータにアクセスされないようにするのに使用します。


## <a name="new-in-preview-released-may---june-2019"></a>プレビュー版の新機能 (リリース日: 2019 年 6 月)

> [!IMPORTANT]
> _プレビュー_の状態では、API やツールを含む機能が予告なしに変更されることがあり、一部の機能が GA 状態に昇格されることはありません。 製品版アプリでは使用しないでください。

### <a name="devices-and-apps"></a>デバイスとアプリ
- Intune [5 月](changelog.md#may-2019)の更新プログラム 
- Intune [6 月](changelog.md#june-2019)の更新プログラム

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta) のデルタ クエリ。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) および [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta) のデルタ クエリとプロパティの追加。

### <a name="group"></a>グループ
[機密度ラベル](/graph/api/resources/assignedlabel?view=graph-rest-beta)を取得して、Office 365 グループの機密データを保護し、コンプライアンス ポリシーに準拠します。 これらのラベルは [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta) オブジェクトで、Microsoft Information Protection 機能の一部として、Microsoft 365 セキュリティ & コンプライアンス センターで管理者により公開されています。 

### <a name="identity-and-access"></a>ID とアクセス
- [アプリケーション](/graph/api/resources/applicationtemplate?view=graph-rest-beta)のインスタンスを取得するか、Azure AD アプリケーション ギャラリーのインスタンスをテンプレートとしてディレクトリに追加します。
- テナントにあるすべての[プロビジョニング イベント](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)のリストを取得します。
- Azure AD 環境で[検出されたユーザーまたはサインインのリスク](/graph/api/resources/riskdetection?view=graph-rest-beta)に関する情報を取得します。 このリスク検出機能は、Azure AD Identity Protection の一部です。

### <a name="mail"></a>メール
[メッセージ](/graph/api/resources/message?view=graph-rest-beta)および** mailFolder **に、[mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) API と、[変更通知](webhooks.md)で [Mail.ReadBasic アクセス許可](permissions-reference.md#mail-permissions)を使用します。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph ツールキット
[Microsoft Graph ツールキット](/graph/toolkit/overview)とは、Microsoft Graph でのデータの認証とアクセスを便宜上提供しているフレームワークにとらわれない Web コンポーネントとヘルパー一式です。 Microsoft Graph ツールキットはプレビュー状態であるため、製品以外のアプリでのみツールキットのプロバイダーとコンポーネントを使用します。

### <a name="sites"></a>サイト
ユーザーは SharePoint サイトを[フォロー](/graph/api/site-follow?view=graph-rest-beta)または[フォロー解除](/graph/api/site-unfollow?view=graph-rest-beta)できます。

### <a name="teamwork"></a>チームワーク
Microsoft Teams の[チャット メッセージ](/graph/api/resources/chatmessage?view=graph-rest-beta)の[画像](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)をホストします。
個人のチームの検出方法の[構成](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)をサポートします。


## <a name="want-to-stay-in-the-loop"></a>常に最新の情報を把握するには?
- Microsoft Graph をサポートするシナリオとは? [Microsoft Graph のユーザーの声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)で新機能を提案および投票します。
- Microsoft Graph コミュニティで活動してください。 毎月の Microsoft Graph コミュニティ コールに[参加](https://aka.ms/microsoftgraphcall)します。
- 
  [Office 365 開発者プログラム](https://developer.microsoft.com/ja-JP/office/dev-program)にサインアップして、無料の Office 365 サブスクリプションに登録して開発を開始してください。


## <a name="see-also"></a>関連項目
- リリース告知と役立つリソースについては、「[Microsoft Graph 開発者ブログ](https://developer.microsoft.com/en-us/graph/blogs/)」を定期的に確認してください。
- Microsoft Graph API の追加機能、[changelog](changelog.md) で API 動作の更新プログラムの詳細を参照してください。
- [以前のリリースの特徴](whats-new-earlier.md)を発見してください。
- 詳細については、「[Microsoft Graph のバージョン管理、サポートと重大な変更の方針](versioning-and-support.md)」を参照してください。

