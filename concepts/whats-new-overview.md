---
title: Microsoft Graph の新機能
description: Microsoft Graph の最新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 13823057cf45dd89ede984748fc8672b9342404a
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "35638958"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph の新機能

Microsoft Graph の一部の新機能は、開発者コミュニティでの要望が高かったことがきっかけとなり提供されるようになりました。 

Microsoft Graph チームでは、お客様のニーズを定期的に評価して API と開発機能の向上を図り、次の順序でそれらを新機能としてリリースします。

1. **_プレビュー_** ステータスでデビューします。 関連するすべての REST API の更新プログラムは、ベータ版のエンドポイントに含まれます(`https://graph.microsoft.com/beta`)。 プレビューの機能は予告なしに変更されることがあります。 製品版アプリにそれらの機能を使用しないでください。 

2. フィードバックで十分に実行可能性が示されるようであれば、 **_一般提供_ (GA)** ステータスに昇格させます。 関連するすべての REST API の更新プログラムは、v1.0 エンドポイントに追加されます (`https://graph.microsoft.com/v1.0`)。 製品版アプリには GA ステータスの機能のみ使用します。

Microsoft Graph の最新機能の特長、[アイデアの共有](#want-to-stay-in-the-loop)方法についてご案内します。 API の更新の詳細については、「changelog」の「[5 月](changelog.md#may-2019)」、「[6 月](changelog.md#june-2019)」、 「[7 月](changelog.md#july-2019)」のセクションを参照してください。 

## <a name="new-and-generally-available-released-may---july-2019"></a>新機能と一般公開 (2019 年 5 月から 7 月にリリース済み)

### <a name="calendar-mail-and-personal-contacts"></a>予定表、メール、個人用連絡先
Exchange 管理者はアプリにアプリケーションのアクセス許可を付与することで、組織内のすべてのメールボックスへのアクセスを許可する既定のアクセス許可の代わりに、[アプリによるアクセスを組織内のメールボックスのサブセットのみに制限](auth-limit-mailbox-access.md)することができます。 このようなアクセス制限は、[予定表](permissions-reference.md#calendars-permissions)、[連絡先](permissions-reference.md#contacts-permissions)、[メールおよびメールボックスの設定](permissions-reference.md#mail-permissions)のアプリに付与されているアプリケーション アクセス許可すべてに適用されます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)を参照してください。

### <a name="example-code-snippets"></a>コード スニペットの例
v1.0 およびベータ リファレンスのすべての API トピックで、C# と JavaScript に加えて Objective-C のコード スニペットが提供されるようになりました。 [イベントを取得](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)するための、Objective-C での例をご覧ください。

### <a name="mail"></a>メール
[メール検索フォルダー](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API を使用して、メッセージを検索し、Outlook のメール検索結果にアクセスできます。 関連する[ブログでのお知らせ](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)を参照してください。

### <a name="postman"></a>Postman
API の動作を学習し、アプリ開発を高速化するために、Graph Explorer の代替として、[Microsoft Graph Postman コレクション](use-postman.md)で Microsoft Graph API をお試しください。

### <a name="tutorials"></a>チュートリアル
[Java コンソール アプリを作成するための新しいチュートリアル](/graph/tutorials/java)を試しに使用して、ユーザーの予定表に関する情報を入手してみてください。

### <a name="user"></a>ユーザー
管理者またはユーザーは、ユーザーに発行されたすべての更新トークンを[取り消す](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)ことができます。 この機能は通常、紛失または盗難にあったデバイスのアプリで組織のデータにアクセスされないようにするために使用されます。


## <a name="new-in-preview-released-may---july-2019"></a>プレビュー版の新機能 (リリース日: 2019 年 5 月 から 7 月)

> [!IMPORTANT]
> _プレビュー_ ステータスの機能 (API やツールを含む) は予告なしに変更されることがあり、一部の機能は GA ステータスに昇格されずに終わります。 プレビュー ステータスの機能は製品版アプリでは使用しないでください。

### <a name="devices-and-apps"></a>デバイスとアプリ
- Intune の[5 月](changelog.md#may-2019)の更新プログラム 
- Intune の[6 月](changelog.md#june-2019)の更新プログラム
- Intune [7 月](changelog.md#july-2019)の更新プログラム

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
[Microsoft Graph ツールキット](/graph/toolkit/overview)とは、フレームワークに依存しない Web コンポーネントおよびヘルパーのセットで、Microsoft Graph でのデータの認証とアクセスを簡便にします。 Microsoft Graph ツールキットはプレビュー ステータスであるため、製品版以外のアプリでのみツールキットのプロバイダーとコンポーネントを使用してください。

### <a name="reports"></a>レポート
セルフサービスによるパスワードのリセットや多要素認証 (MFA) など、組織内のユーザーによって導入される[認証方法に関するレポート](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta)を取得します。

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

