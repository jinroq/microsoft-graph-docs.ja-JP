---
title: Outlook 個人用連絡先 API の概要
description: Outlook の連絡先を利用すると、個人用連絡先のデータを保存することができます。これは、Office 365 の Outlook メッセージング ハブの一部です。 Outlook により、メールの管理、会議のスケジュール管理、組織内のユーザーに関する情報の検索、オンライン会話の開始、ファイルの共有、およびグループでの共同作業をすることができます。
author: angelgolfer-ms
ms.openlocfilehash: bccf32fd0cc3022a146e16590d915c4b85d60127
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347517"
---
# <a name="outlook-personal-contacts-api-overview"></a>Outlook 個人用連絡先 API の概要

Outlook の連絡先を利用すると、個人用連絡先のデータを保存することができます。これは、Office 365 の Outlook メッセージング ハブの一部です。 Outlook により、メールの管理、会議のスケジュール管理、組織内のユーザーに関する情報の検索、オンライン会話の開始、ファイルの共有、およびグループでの共同作業をすることができます。

## <a name="why-integrate-with-outlook-personal-contacts"></a>Outlook 個人用連絡先を統合する理由

### <a name="complement-messaging-and-calendaring-scenarios-for-hundreds-of-millions-of-customers"></a>何億人もの顧客を対象としたメッセージングと予定管理のシナリオを補完

Outlook は、何億人という消費者および何千万という組織ユーザーによりメール クライアントとして選ばれています。 Outlook 内の連絡先データのための便利な統合保存場所をユーザーに提供する連絡先は、メッセージングおよび予定管理のための補助機能を提供します。 開発者にとっては、[メール](outlook-mail-concept-overview.md)や[予定表](outlook-calendar-concept-overview.md)の豊富な機能を利用することにより、ユーザーの連絡先データに関するシナリオをさらに充実させることができます。


### <a name="automate-contact-organization"></a>連絡先の整理を自動化

連絡先 API を利用することにより、顧客が Outlook により自分で情報を整理するのに伴って、顧客情報を常に整理された状態に維持することができます:

- 顧客エクスペリエンスに対するのと同じように、[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスを作成し、それを [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) オブジェクトに割り当てることができます。
- 連絡先 API を利用すれば、カテゴリ連絡先と共に、イベント、メッセージ、タスク、およびグループ投稿を一貫した方法で割り当てることができ、情報の整理や検出のための機能がさらに充実します。 加えて、[カテゴリのユーザー マスター リストを定義](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0)することができ、それによりクリエイティブなシナリオがさらに豊富になります。
- フォローアップのためのフラグを[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)に設定できます。 (現時点で Microsoft Graph のフラグの機能は[プレビュー段階](versioning-and-support.md#beta-version)です。)


### <a name="share-contact-information"></a>連絡先情報を共有する

連絡先 API を利用することにより、サインイン ユーザー、またはサインイン ユーザーと連絡先を共有または委任しているユーザーの連絡先項目を入手することができます。 たとえば、Garth が連絡先フォルダーを John と共有している場合、または Garth がアクセスを John に委任している場合、John からの[アクセス許可委任](permissions-reference.md#delegated-permissions-application-permissions-and-effective-permissions)により Garth が共有に設定している予定表およびコンテンツにも読み取りアクセスが可能になります。


### <a name="leverage-people-api-in-microsoft-graph-to-make-better-use-of-all-people-data"></a>Microsoft Graph の連絡先 API 利用であらゆる連絡先データをさらに有効利用

Outlook [連絡先](/graph/api/resources/contact?view=graph-rest-1.0)のための典型的な CRUD 操作を使用することにより、連絡先を作成したり管理したりすることができます。 Microsoft Graph の一部として、[連絡先 API](people-example.md) を使用することができます。それにより、ユーザーの Outlook 連絡先、ソーシャル ネットワーク、組織ディレクトリ、最近の通信での連絡先情報を調べることができ、ユーザーにとって最も関連性の高い情報源すべてから連絡先情報を得ることができます。 連絡先検出シナリオでは、インテリジェントなこの付加機能を活用してください。


### <a name="take-advantage-of-other-shared-features-and-conveniences-in-microsoft-graph"></a>Microsoft Graph でのその他の共有機能や便利機能の活用

- **連絡先**エンティティでは、Exchange Online や Azure Active Directory に保存されたユーザーの写真と同じ [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-1.0) エンティティとして実装されている連絡先写真がサポートされています。 これにより、連絡先とユーザー プロファイル写真の間で変換するというオーバーヘッドを回避できます。
- [変更通知](/graph/api/resources/webhooks?view=graph-rest-1.0)のサブスクリプションを取得し、連絡先および連絡先フォルダーに対する[変更を追跡](delta-query-overview.md)することにより、アプリのローカル ストアの同期を維持することができます。
- 連絡先インスタンスのアプリ ストレージを[オープン拡張](extensibility-overview.md#open-extensions)として拡張したり、厳密に型指定されたカスタム データを連絡先スキーマに[スキーマ拡張](extensibility-overview.md#schema-extensions)として追加したりすることができます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Outlook 連絡先 API](/graph/api/resources/contact?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Outlook 連絡先 API](/graph/api/resources/contact?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

- [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fcontacts&version=v1.0) で連絡先サンプル クエリを選択して試行する。 左側の列の **[サンプルをさらに表示]** を選択します。 メニューを使用して **[個人用連絡先]** をオンにします。
- 以下について調べます。
  - [Outlook リソースの不変識別子の取得](outlook-immutable-id.md)
  - [共有の連絡先の取得](outlook-get-shared-contacts-folders.md)
- Outlook の[連絡先 API](/graph/api/resources/contact?view=graph-rest-1.0) リファレンスをご確認ください。
