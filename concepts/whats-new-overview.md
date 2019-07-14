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

Microsoft Graph の一部の新機能は、開発者コミュニティでの要望が高かったことがきっかけとなり提供されるようになりました。 

そこで、新機能の典型的なライフ サイクル、Microsoft Graph の最新機能、[アイデアの共有](#want-to-stay-in-the-loop)方法についてご案内します。

## <a name="life-cycle-of-a-feature"></a>機能のライフ サイクル

Microsoft Graph サービスの所有者は、機能のアイデアや顧客のニーズを定期的に評価し、サポートする新しいシナリオを選択します。 新機能を作成するために、REST API を追加または更新することがあります。 API 構文は変えずに、機能の動作を拡張する場合があります。 あるいは、学習または開発環境が改善される場合もあります。

ほとんどの場合、サービス所有者は次の順序で新機能をリリースします。

1. 機能は「**_プレビュー_**」ステータスで導入されます。機能の動作が予告なく変更される可能性があることを意味します。 所有者は、ベータ版エンドポイント (`https://graph.microsoft.com/beta`) で関連する REST API の追加や更新プログラムを公開します。 製品版アプリでは、プレビュー機能およびそれらの機能の API を使用しないでください。

2. サービスの所有者が十分な量のフィードバックを受け取り、検討中の機能が実現可能であると判断した場合、所有者は機能を「**_一般提供_」(GA)** ステータスに昇格させます。 所有者は、関連する API の追加や変更を v1.0 エンドポイント (`https://graph.microsoft.com/v1.0`) に加えます。 GA ステータスの機能 (その機能の API を含む) は、製品版アプリで使用できます。

以下のセクションでは、2019 年 5 月と 6 月の新機能について説明します。 API の更新の詳細については、「changelog」の「[5 月](changelog.md#may-2019)」と「[6 月](changelog.md#june-2019)」のセクションを参照してください。 

## <a name="new-and-generally-available-released-may---june-2019"></a>新機能と一般公開 (2019 年 5 月～6 月にリリース済み)

### <a name="calendar-mail-and-personal-contacts"></a>予定表、メール、個人用連絡先
Exchange 管理者は、組織内のすべてのメールボックスへのアクセスを許可する既定のアクセス許可ではなく、[アプリによるアクセスを組織内のメールボックスのサブセットのみに制限](auth-limit-mailbox-access.md)するようにアプリケーション アクセス許可をアプリに付与できます。 このようなアクセス制限は、アプリに付与されている[予定表](permissions-reference.md#calendars-permissions)、[連絡先](permissions-reference.md#contacts-permissions)、[メールおよびメールボックスの設定](permissions-reference.md#mail-permissions)についてのアプリケーション アクセス許可に適用されます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)を参照してください。

### <a name="example-code-snippets"></a>コード スニペットの例
v1.0 およびベータ リファレンスのすべての API トピックで、C# と JavaScript に加えて Objective-C のコード スニペットが提供されるようになりました。 [イベントを取得](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)するための、Objective-C での例をご覧ください。

### <a name="mail"></a>メール
[メール検索フォルダー](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API を使用して、メッセージを検索し、Outlook のメール検索結果にアクセスできます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)を参照してください。

### <a name="postman"></a>Postman
API の動作を学習し、アプリ開発を高速化するために、Graph Explorer の代替として、[Microsoft Graph Postman コレクション](use-postman.md)で Microsoft Graph API をお試しください。

### <a name="tutorials"></a>チュートリアル
[Java コンソール アプリを作成するための新しいチュートリアル](/graph/tutorials/java)を試しに使用して、ユーザーの予定表に関する情報を入手してみてください。

### <a name="user"></a>ユーザー
管理者またはユーザーは、ユーザーに発行されたすべての更新トークンを[取り消す](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)ことができます。 この機能は通常、紛失または盗難にあったデバイス上のアプリが組織のデータにアクセスできないようにする目的に使用します。


## <a name="new-in-preview-released-may---june-2019"></a>プレビュー版の新機能 (リリース日: 2019 年 6 月)

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
- テナントにあるすべての[プロビジョニング イベント](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)のリストを取得できます。
- Azure AD 環境で[検出されたユーザーまたはサインイン リスク](/graph/api/resources/riskdetection?view=graph-rest-beta)に関する情報を取得できます。 このリスク検出機能は、Azure AD Identity Protection の一部です。

### <a name="mail"></a>メール
[mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) API と[メッセージ](/graph/api/resources/message?view=graph-rest-beta)および **mailFolder** に関する[変更通知](webhooks.md)で [Mail.ReadBasic アクセス許可](permissions-reference.md#mail-permissions)を使用できます。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph ツールキット
[Microsoft Graph ツールキット](/graph/toolkit/overview)とは、フレームワークに依存しない Web コンポーネントおよびヘルパーのセットで、Microsoft Graph でのデータの認証とアクセスを簡便にします。 Microsoft Graph ツールキットはプレビュー ステータスであるため、ツールキットのプロバイダーとコンポーネントは製品版以外のアプリでのみ使用してください。

### <a name="sites"></a>サイト
ユーザーは SharePoint サイトを[フォロー](/graph/api/site-follow?view=graph-rest-beta)または[フォロー解除](/graph/api/site-unfollow?view=graph-rest-beta)できます。

### <a name="teamwork"></a>チームワーク
Microsoft Teams の[チャット メッセージ](/graph/api/resources/chatmessage?view=graph-rest-beta)の[画像](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)をホストできます。
プライベート チームの検出方法の[構成](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)がサポートされます。


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

