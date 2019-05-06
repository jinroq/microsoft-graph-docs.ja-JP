---
title: Outlook メール API の概要
description: Outlook は、Office 365 のメッセージング通信ハブです。 連絡先の管理、会議のスケジュール管理、組織内のユーザーに関する情報の検索にも使用できます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 86f7506ec06325657465a5762261a061bf0ad575
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2019
ms.locfileid: "33440067"
---
# <a name="outlook-mail-api-overview"></a>Outlook メール API の概要

Outlook は、Office 365 のメッセージング通信ハブです。 これにより、連絡先の管理、会議のスケジュール管理、組織内のユーザーに関する情報の検索、オンライン会話の開始、ファイルの共有、およびグループでの共同作業をすることができます。

## <a name="why-integrate-with-outlook-mail"></a>Outlook メールと統合する理由

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>豊富な機能を統合して何億というユーザーに達する

Outlook を統合するなら、多くのユーザーの好む豊かなエクスペリエンスを取り入れることになります。それは、メール、[連絡先](outlook-contacts-concept-overview.md)、[予定表](outlook-calendar-concept-overview.md)のための直感的で一貫したエクスペリエンスであり、モバイル、Web、およびデスクトップのどのデバイス上でも利用可能です。

[Microsoft Graph](overview.md) を使用することにより、アプリを 1 回だけ作成することにより Outlook と統合することができ、Outlook をメール クライアントとして選んでいる何億人という消費者、何千万という組織ユーザーに達することができます。 メール シナリオを中心としたアプリを作成したり、Outlook および 非 Outlook の他のリレーションシップ、リソース、およびインテリジェンスの宝庫に接続したり、Microsoft クラウドによってサポートされるシナリオを実現したりすることができます。

### <a name="automate-message-organization-and-processing"></a>メッセージの整理と処理を自動化する

多くのユーザーは、Outlook で情報を整理するのを好んでいます。 Microsoft Graph により、それらの機能をアプリ開発者が利用することができ、情報の発見作業を最適化し、効率や生産性を向上させるユーザー ワークフローを構築することができます:

- ユーザーは、さまざまな方法でメッセージを整理できます。メッセージを全部受信トレイに入れたまま検索する人もいれば、複数のフォルダーにメッセージを分類保存する人もいます。 フラットな整理方法とフォルダー ベースの整理方法の両方をサポートする Outlook の柔軟で直感的なアプローチがユーザーに好まれています。 アプリでは、特定のフォルダー内のメッセージまたはユーザーのメールボックス全体のメッセージに対して[フィルター処理、検索、またはソート](query-parameters.md)を便利に実行することができます。

- Outlook では、名前と色によってカテゴリが区別されます。 カテゴリを利用することによりユーザーは、メッセージにタグを付けて、整理や情報発見の作業をさらに便利なものにすることができます。 アプリでは、[ユーザーのカテゴリ マスター リストにアクセスしたり定義したり](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0)できます。 さらにそのリストは、Outlook のメッセージ、またイベント、連絡先、タスク、およびグループ投稿を通じて共有され、アプリ開発者にとってクリエイティブなシナリオの可能性をもたらします。 たとえば、オンライン研修業者であれば、電子メール、コース イベント、およびフォローアップ課題を、ユーザーが登録しているコースごとに色分けすることができます。

- さらに、アプリのユーザーは、メッセージ (あるいは、イベントまたはタスク) の重要度を変更したり、メッセージにフォローアップ用のフラグを付けたりすることができます。 (現時点で Microsoft Graph のフラグの機能は[プレビュー段階](versioning-and-support.md#beta-version)です。)

- ルール API を利用すれば、メッセージの整理がさらに上のレベルになります。 アプリでは、[受信トレイ ルール](/graph/api/resources/messagerule?view=graph-rest-1.0)をセットアップすることにより、受信メッセージを迅速に処理し、メールが乱雑な状態になるのを軽減できます。 たとえば、アプリにより、メッセージの件名に特定のキーワードが含まれている場合にメッセージを別のフォルダーに移動したり、後でそれに対応する作業を容易にするためにカテゴリや重要度を割り当てたりすることができます。

### <a name="write-smarter-apps-that-leverage-intelligence"></a>インテリジェンスを活用した高度なアプリを作成する

Microsoft Graph を利用することにより、アプリ ユーザーに対してコンテキスト データを提案することができます:

- [優先受信トレイ](/graph/api/resources/manage-focused-inbox?view=graph-rest-1.0)および [@-メンション (プレビュー)](/graph/api/message-get?view=graph-rest-beta#request-2) を統合し、アプリ ユーザーが気になっているものを最初に読み、返信できるようにする。

- メッセージ作成中に[メール ヒント](/graph/api/resources/mailtips?view=graph-rest-1.0)をチェックして、受信者に関する有用な情報を得る (受信者が自動返信を送信中なのか、あるいはメールボックスがいっぱいなのかなど)。 メール ヒントは、アプリに対して特定の条件を警告することにより、フォローアップのアクションの効率を上げることができます。

- [連絡先 API](people-example.md) の利用により、アプリの中で連絡先を選択するなど、対話式のコントロールが提供されます。 連絡先 API では、ユーザーの通信および共同作業のパターン、そしてビジネス上の付き合いに基づいて、ユーザーに最も関係の深い連絡先を提案することができます。

- アプリ ユーザーに対して、メッセージ作成中に添付ファイルに関連して、気の利いたファイル選択機能を提供したり、最近利用したファイルを提案したりする。 [Insights (プレビュー)](/graph/api/resources/insights?view=graph-rest-beta) では、高度な分析機能を使用することにより、ユーザーの周辺で頻繁に使用されるファイル、最近ユーザーが表示または編集したファイル、あるいはそのユーザーと共有したファイルについての提案がなされます。


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>アプリ データをリソースまたはリソース インスタンスに保存する

アプリでは、データを外部データ ストアに保存するために、データの管理とアクセスのためのオーバーヘッドが発生することが少なくありません。 Microsoft Graph では、新しいメッセージを[作成](/graph/api/user-post-messages?view=graph-rest-1.0#request-2)または[送信](/graph/api/user-sendmail?view=graph-rest-1.0#request-2)するとき、あるいはメッセージに返信するときに、アプリのデータをインターネット メッセージ ヘッダーとして追加するだけで対処できます。

カスタム データを追加して、そのデータを後で更新する必要がある場合、[カスタム データを個別のリソース インスタンスに格納](extensibility-overview.md#open-extensions)できます。 必要に応じて、スキーマを拡張してカスタム プロパティを追加し、型指定されたデータを Microsoft Graph のリソースに格納するという方法も使えます。 そのような[スキーマ拡張](extensibility-overview.md#schema-extensions)を、検出可能また共有可能なものにすることができます。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

- [Microsoft Graph v1.0 の Outlook メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版の Outlook メール API](/graph/api/resources/mail-api-overview?view=graph-rest-beta)


## <a name="next-steps"></a>次の手順

- [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) で Outlook メール サンプル クエリを選択して試行する。 左側の列の **[サンプルをさらに表示]** を選択します。 メニューを使用して **Outlook メール** をオンにします。
- 以下について調べます。

  - [メッセージの作成と送信](outlook-create-send-messages.md)
  - [メッセージの整理方法](outlook-organize-messages.md)
  - [メッセージの MIME コンテンツを取得する](outlook-get-mime-message.md)
  - [共有メッセージを取得する](outlook-share-messages-folders.md)
  - [Outlook リソースの不変識別子の取得](outlook-immutable-id.md)
  - [別のユーザーからのメールを送信する](outlook-send-mail-from-other-user.md)方法

- Microsoft Graph v1.0 での[メール API の使用](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)について調べる。


